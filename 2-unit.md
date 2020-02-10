# 🔬 2 - Unit: Pruebas unitarias

## Pruebas sobre el código hecho

---

## 🦄 Prueba de artefactos individuales de código, tal como **funciones o clases.**

## 🆗 Suministra una entrada y comprueba que retorne **la salida o el efecto esperado.**

## 👥 Comprueba que los módulos desarrollados cumplen los **requisitos funcionales.**

## 📖 Se escriben sobre código conocido, luego son de **caja blanca.**

## 📓 Suele bastar con la interface pública; como una **caja gris.**

---

## 🛠 Tools

### [Jest](https://jestjs.io/)

### Alternatives

#### [Karma](https://karma-runner.github.io/2.0/index.html)

#### [Jasmine](https://jasmine.github.io/)

---

## 🚀 Install and config

```bash
yarn add -D @babel/core @babel/preset-env
yarn add -D jest @types/jest babel-jest
# configure babel.config.js
# configure jest.config.js
```

```json
// package.json
{
  "jest": "jest",
  "test": "jest --watch -o",
}
```

---

## 🔬 Unit tests

> minimal _hello testing world_ outline

```js
/*
FEATURE:    Purpose of the Subject Under Test
As a:       user of the SUT
I want to:  do something
So:         I achieve a goal.
*/

// Scenario: a real user situation
describe('GIVEN: a context', () => {
  // Arrange
  const sut = null;
  describe('WHEN: some conditions', () => {
    const input = null;
    //Act
    const actual = null; // = sut( input ) ; = sut().method(input);
    test('THEN: expect some output', () => {
      const expected = null;
      // assert
      expect(actual).toEqual(expected);
    });
  });
});

```
