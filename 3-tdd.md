# 2 - TDD: Test Driven Development

**Código hecho para pasar las pruebas:**

- Escribe una prueba que falle. RED ❌
- Escribe el código imprescindible para pasar la prueba. GREEN ✅
- Mejora el código con tranquilidad. REFACTOR ✅ ✅

## Tools

- [Jest](https://jestjs.io/)

### Alternatives

- [Karma](https://karma-runner.github.io/2.0/index.html)

- [Jasmine](https://jasmine.github.io/)

## Teacher Sample

> See history commits

- [tdd-hamming-dna](https://github.com/AcademiaBinaria/unit-test/blob/master/tdd/teacher/hamming-dna.spec.js)

#### Funcional tests already done

- **FEATURE:**    Calculate the Hamming Distance between two DNA strands.
  - _Aa a:_       biologist studying cell divisions
  - _I want to:_  compare two strands of DNA and count the differences between them
  - _So:_         I can see how many mistakes occurred.

### SUT

- [hamming-dna.js](https://github.com/AcademiaBinaria/unit-test/blob/master/tdd/teacher/hamming-dna.js)

## Student Practice

### SUT

- [leap-year.js](https://github.com/AcademiaBinaria/unit-test/blob/master/tdd/student/leap-year.spec.js)

### Functional tests to de done

#### Beginner

- **FEATURE:**:   Given a year, report if it is a leap year.
  - _As a:_       calendar printer
  - _I want to:_  know if February has 28 or 29 days
  - _So:_         I can print my calendars
    - **Scenario:** given a year


#### Boss

- **Scenario:** given anything...


## Advanced real scenario

- [exchange-calculator.spec.js](https://github.com/AcademiaBinaria/unit-test/blob/master/tdd/real/exchange-calculator.spec.js)