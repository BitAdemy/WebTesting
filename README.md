---
marp: false
---

# 🧪 Web Testing

>"Codifica como si la persona que mantendrá tu código fuera un psicópata violento que sabe dónde vives."
>
> -- ✍️ **Martin Golding**

---

## 🎯 Objetivos

- Conocer la **terminología** y la filosofía de los distintos tipos de pruebas.
- Comprobar funcionalidades con pruebas **_end to end_** de aplicaciones web.
- Refactorizar código **_legacy_** con la tranquilidad de las pruebas unitarias.
- Crear nuevo código bajo el paradigma **_Test Driven Development_**.

## 👨‍💻 A quién va dirigido

- Programadores de aplicaciones con experiencia.
- Conocimientos de tecnología web: HTML y JavaScript.

---

## 💻 Material necesario

- Editor de código y navegador modernos.
  - Recomendados _VSCode_ y _Chrome_
- _Node_ versión 12
- Capacidad para instalar paquetes desde _npm_


<!-- ### 🔗 Enlaces

#### Laboratorios

- [E2E Puppeteer](https://github.com/LabsAdemy/WebTesting_e2e-puppeteer_Labs)

- [E2E Cypress](https://github.com/LabsAdemy/WebTesting_e2e-functional_cypress_Labs)

- [Unit Jest](https://github.com/LabsAdemy/WebTesting_unit_Labs/tree/master/src/unit)

- [TDD Jest](https://github.com/LabsAdemy/WebTesting_unit_Labs/tree/master/src/tdd)

#### [Tutorial Documentación](https://www.bitademy.com/tutorial/web-testing/contenido/) -->

---

## 🏁 Introducción

- Las pruebas del software han sido **ignoradas y hasta despreciadas** por muchos.

- Otros las ven como una _absurda obligación_.

- No más _negacionismo_!
  - Hay relación directa entre **calidad y pruebas**.

---

### ✅ La detección temprana de **errores**,

### ✅ la validación de las **funcionalidades**

### ✅ la mejora en el **diseño** del código.



## 📈 **Las pruebas ahorran dinero.**

---

## 🔬 Hacer pruebas

### Proceso
  - Aprendizaje
  - Adopción

### En este curso te mostraré
  - Los fundamentos
  - Las técnicas

### Al finalizar podrás:
  - Incluirlos **inmediatamente**
  - **Mejorar la calidad** de tus programas.

---

### 🛠 Herramientas

#### **JavaScript** Tienes todo lo necesario. Puedes hacer pruebas sin framework.

  <!-- - Ya tienes todo lo que necesitas. Puedes hacer pruebas sin ningún framework. -->

#### **Puppeteer** Manipular el navegador. Ideal para _e2e_ no funcional

  <!-- - Manipular y simular actividad con el navegador. Ideal para _e2e_ no funcional. -->

#### **Lighthouse** comprobación de rendimiento, SEO...

  <!-- - Comprobación del rendimiento, el SEO y buenas prácticas web. -->

#### **Cypress** pruebas funcionales de integración o _e2e_

  <!-- - Framework de pruebas funcionales de integración o _e2e_. -->

#### **Jest** _zero configuration_. Ideal para _unit testing_ y _TDD_

  <!-- - Framework _zero configuration_. Ideal para _unit testing_ y _TDD_. -->

<!-- ---

### Otros

- **[Playwright](https://github.com/microsoft/playwright)** automatizador de diversos navegadores al estilo Puppeteer.

- **[Karma](https://karma-runner.github.io/latest/index.html)** es un ejecutador de pruebas muy interesante para integración continua.

- **[Jasmine](https://jasmine.github.io/)** muy completo y bueno para user-behavior por su expresividad

- **[Mocha](https://mochajs.org/)** muy utilizado para NodeJS.

- **[Chai](https://www.chaijs.com/)** librería muy adecuada para BDD con NodeJS. -->

---

### ✅ [0 - TEST Software que funciona.](https://www.bitademy.com/tutorial/web-testing/software-que-funciona)

#### 🔀 [Tipos de test](https://www.bitademy.com/tutorial/web-testing/tipos-de-pruebas)

#### 👨🏼‍🏫 [Filosofía y patrones](https://www.bitademy.com/tutorial/web-testing/filosofia-y-patrones)

---
### ✅ [1 -Primeras pruebas.]()

#### 🧪 [Pruebas de funciones puras](https://www.bitademy.com/tutorial/web-testing/functional/limpieza-de-pruebas)

#### 🧪 [Pruebas de integración de clases](https://www.bitademy.com/tutorial/web-testing/functional/limpieza-de-pruebas)

#### 🧪 [Pruebas unitarias](https://www.bitademy.com/tutorial/web-testing/functional/limpieza-de-pruebas)

#### 🧪 [TDD Pruebas antes que el código](https://www.bitademy.com/tutorial/web-testing/functional/limpieza-de-pruebas)

---
### 🌐 [2 - E2E: Pruebas web de principio a fin.](https://www.bitademy.com/tutorial/web-testing/e2e)

#### 🎭 [**Puppeteer** para pruebas de contenido y visualización](https://www.bitademy.com/tutorial/web-testing/e2e/pruebas-de-aplicaciones-web-con-puppeteer)

#### 🚢 [**Lighthouse** para pruebas de rendimiento web](https://www.bitademy.com/tutorial/web-testing/e2e/pruebas-de-rendimiento-web-con-lighthouse)

#### 🚢 [Pruebas de un API REST]()

---

### 🌲 [3 - Pruebas funcionales de aplicaciones web con **Cypress**](https://www.bitademy.com/tutorial/web-testing/functional)

#### 🎪 [Simulando el comportamiento del usuario](https://www.bitademy.com/tutorial/web-testing/functional/pruebas-de-comportamiento)

#### 🤖 [Automatización e integración continua](https://www.bitademy.com/tutorial/web-testing/functional/pruebas-de-comportamiento)
---

### 🔬 [4 - Pruebas unitarias con **Jest**](https://www.bitademy.com/tutorial/web-testing/unit)

#### 🕵🏼‍♂️ [Pruebas de integración]

#### 🕵🏼‍♂️ [Pruebas unitarias con dobles](https://www.bitademy.com/tutorial/web-testing/unit/pruebas-con-espias-y-dobles)

#### 🏇🏼 [Pruebas de código asíncrono](https://www.bitademy.com/tutorial/web-testing/unit/pruebas-de-codigo-asincrono)

---

### 🧬 [5 - TDD: desarrollo guiado por las pruebas](https://www.bitademy.com/tutorial/web-testing/tdd)

#### ♻ [El ciclo virtuoso.](https://www.bitademy.com/tutorial/web-testing/tdd/mejores-resultados-y-mejor-diseno)

#### 📈 [Mejores resultados y mejor diseño.](https://www.bitademy.com/tutorial/web-testing/tdd/mejores-resultados-y-mejor-diseno)
---

>"Los desarrolladores no tienen que justificar las **pruebas** y la refactorización; porque esas disciplinas aumentan su eficiencia y su **productividad**."
>
> -- ✍️ **Robert C. Martin**
---

<!-- [![bit_ademy](./assets/bit_ademy.png)](https://bitademy.com) -->
<!-- [![vitae](./assets/vitae.png)](https://vitaedigital.com) -->


✍️ **Alberto Basalo**

## 2020