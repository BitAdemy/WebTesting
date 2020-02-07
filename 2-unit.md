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


---

> Copy from : https://github.com/AcademiaBinaria/unit-test
>
> To: https://github.com/LabsAdemy/WebTesting_unit_Labs

---

## Teacher Sample

- [unit-highscores](https://github.com/AcademiaBinaria/unit-test/blob/master/teacher/high-scores.spec.js)

#### Funcional tests already done

- **FEATURE:**    Manage a game player's High Score list.
  - _Aa a:_       player with an array of scores
  - _I want to:_  to get the scores ordered, my last, my best, and my top three scores
  - _So:_         I can track my progress


### SUT

- [high-scores.js](https://github.com/AcademiaBinaria/unit-test/blob/master/teacher/high-scores.js)

## Student Practice

### SUT

- [triangle.js](https://github.com/AcademiaBinaria/unit-test/blob/master/student/triangle.js)

### Functional tests to de done

#### Beginner

- **FEATURE:**: Determine if a triangle is equilateral, isosceles, or scalene.
  - _As a_ math student
  - _I want to_ check the kind of any triangle
  - _So_ I can learn about its geometry
    - **Scenario:** I have a valid triangle with three sides
    - **Scenario:** I have a valid triangle with three equal sides
    - **Scenario:** I have a valid triangle with no equal sides


#### Boss

- **Scenario:** I have an invalid triangle
