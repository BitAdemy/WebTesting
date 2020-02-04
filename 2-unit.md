# 2 - Unit: Pruebas unitarias

**Test unitarios:**

Prueba de unidades individuales de código, tal como **funciones o clases**, mediante el suministro de una entrada y comprobando que la salida sea la esperada.

Las pruebas unitarias permiten comprobar que los módulos desarrollados cumplen los **requisitos funcionales**.

Estas pruebas se escriben conociendo el módulo que se va probar, en ese sentido son de **caja blanca**. Pero, sólo tenemos que probar la interface pública exportada; podríamos decir que son de **caja gris...**


## Tools

- [Jest](https://jestjs.io/)

### Alternatives

- [Karma](https://karma-runner.github.io/2.0/index.html)

- [Jasmine](https://jasmine.github.io/)

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
