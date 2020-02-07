# 2 - Unit: Pruebas unitarias

**Pruebas sobre el código hecho:**

- Prueba de artefactos individuales de código, tal como **funciones o clases**. 🦄

- Suministra una entrada y comprueba que la salida sea la esperada. 🆗

- Comprueba que los módulos desarrollados cumplen los **requisitos funcionales**. 👥

- Se escriben conociendo el módulo que se va probar, en ese sentido son de **caja blanca**. 📖

- Suele ser suficiente probar la interface pública; podríamos decir que son de **caja gris**...📓


## Tools

- [Jest](https://jestjs.io/)

### Alternatives

- [Karma](https://karma-runner.github.io/2.0/index.html)

- [Jasmine](https://jasmine.github.io/)


## Install and config



## Unit tests

> minimal hello world outline

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
