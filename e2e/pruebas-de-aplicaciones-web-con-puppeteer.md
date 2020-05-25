---
marp: true
---

# 🎭 Pruebas de aplicaciones web con Puppeteer---

## Puppeteer para comprobación de existencia, navegación, tamaño, velocidad y otras métricas.

> _"Hacer las pruebas de existencia y rendimiento al terminar el desarrollo o tras las pruebas funcionales es como tomar el pulso o hacer una analítica a un paciente que ya está muerto."_
>
> -- ✍️ **Scott Barber**

---

# _Puppeteer:_  Pruebas básicas.

## Preparado y automatizado

### Sencillo
### Barato
### Frecuente

---

## Puppeteer y Node

- Un script Node que tome como dependencia a [Puppeteer](https://pptr.dev/).

- Con los comandos `assert` propios de Node.

- Estructura con la _triple A_ **Arrange-Act-Assert**.
---

### Arrange

- Configurar y preparar: _Arrange_

```js
async function arrangeBrowser() {
  console.info(`arranging browser `);
  const browser = await puppeteer.launch({
    headless: true,
    defaultViewport: { width: 1920, height: 1080 }
  });
  const pagePuppet = await browser.newPage();
  return { browser, pagePuppet };
}
```

---

- Intento lo que debería ocurrir

```js
module.exports = async function itShouldExist(pagePuppet) {
  let errors = 1;
  const inputPageUrl = 'https://www.bitademy.com';
  console.info(`GIVEN the url: ${inputPageUrl}`);
  try {
    console.info(`  WHEN is visited`);
    await pagePuppet.goto(inputPageUrl, { waitUntil: 'networkidle2' });
    console.info(`    THEN it Should Exist a page: ${inputPageUrl}`);
    errors = 0;
  } catch (error) {
    console.warn({ error });
  }
  assertTrue(errors == 0, `Could not visit the url: ${inputPageUrl}`);
  return errors;
};
```

---

### _Given, when, then_.

```
async function itShouldHaveTitle(pagePuppet) {
  console.info(`GIVEN a page`);
  const expected = 'bitAdemy';
  ...
}
```

---

### Act

- Actuar para obtener la realidad: `actual`.

```js
async function itShouldHaveTitle(pagePuppet) {
  ...
  console.info(`  WHEN we get its title`);
  const actual = await actGetTitle(pagePuppet);
  ...
}
async function actGetTitle(pagePuppet) {
  return await pagePuppet.title();
}
```

---

### Assert

Comprobar que algo es cierto `assert`.

```js
async function itShouldHaveTitle(pagePuppet) {
  ...
  console.info(`    THEN it Should Have Title: ${expected}`);
  return assertEqual(actual, expected);
}
function assertEqual(actual, expected) {
  try {
    assert.strictEqual(actual, expected);
    console.info(`      🟩 SUCCESS`);
    return 0;
  } catch (error) {
    console.info(`      🔴 FAIL: expected ${error.expected} but got ${error.actual} `);
    return 1;
  }
}
```

---

### After

- Limpiar al terminar: `after`.

```js
async function afterAll(browser, numErrors) {
  await browser.close();
  if (numErrors) {
    console.warn(`🔴 FAIL: there are ${numErrors} site errors`);
  } else {
    console.info('🟩 SUCCESS: all tests completed successfully');
  }
  process.exit(numErrors);
}
```

---

### Interacción

- Simular acciones de usuario

  - Navegación
  - Escritura
  - Click

- Si se complica... **[Cypress](https://www.cypress.io/)**

---

Un ejemplo de suscripción a una newslwetter

```js
module.exports = async function itShouldAllowSubscribe(pagePuppet) {
  let errors = 1;
  console.info(`GIVEN a page with a subscribe form `);
  try {
    console.info(`  WHEN we select the input `);
    await actSelect(pagePuppet, '#MERGE0');
    console.info(`  AND WHEN we type at the selected input `);
    await actType(pagePuppet, 'puppet@bitademy.com');
    console.info(`  AND WHEN we click on the subscribe button `);
    await actClick(pagePuppet, '#subscribe-form > button');
    console.info(`    THEN it Should Allow Subscribe`);
    errors = 0;
  } catch (error) {
    console.warn({ error });
  }
  assertTrue(errors == 0, `Could not complete subscribe process`);
  return errors;
};
```
---

```js
async function actSelect(pagePuppet, selector) {
  await pagePuppet.evaluate(function (selector) {
    return document.querySelector(selector).scrollBy(0, 10);
  }, selector);
  await pagePuppet.focus(selector);
}

async function actType(pagePuppet, value) {
  await pagePuppet.keyboard.type(value);
}

async function actClick(pagePuppet, selector) {
  await pagePuppet.click(selector);
}
```

---

### Imagen

- **capturar instantáneas y guardarlas**
- **distintas resoluciones o simuladores de dispositivos**.


```js
module.exports = async function takeScreenshot(pagePuppet) {
  const timeStamp = new Date().getTime();
  const shotPath = path.join(process.cwd(), 'images', `${timeStamp}.png`);
  await pagePuppet.screenshot({
    path: shotPath,
    fullPage: true
  });
};
```

--

> En [el laboratorio](https://github.com/LabsAdemy/WebTesting_e2e-puppeteer_Labs) tienes más ejemplos de lo que es capaz _Puppeteer_. Y si aún quieres más puede mirar este otro repositorio aún más completo [AtomicBuilders/muon](https://github.com/AtomicBuilders/muon)
