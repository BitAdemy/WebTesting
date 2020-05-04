# 🔀 Tipos de Pruebas

Hay una prueba para cada situación.

> _"Escribe tests. No demasiados. Principalmente de integración."_
>
> ✍🏼 Kent C. Dodds

---

Si empiezo con esta frase es para introducir la idea de que no hay un sólo tipo de test. Y dejar caer que no hay volverse locos probado código. Es mejor empezar poco a poco, pero empezar. Si ya has empezado, entonces avanza un poco más.

En cualquier caso te vendrá bien un repaso de conceptos básicos y nomenclatura.

## Tipos de Pruebas

### 🤖 Manuales -> Programadas

- ❌ Dependemos de las personas

- ✔️ Se pueden configurar y lanzar automáticamente

### ⚖ Técnicas -> Funcionales

- ⚪ Se puede comprobar el rendimiento, la seguridad, usabilidad...

- ✔️ La función del software, su utilidad.

### 🔎 Unitarias -> De integración -> De inicio a fin

- ✔️ **unitarias**: Pruebas de caja blanca que verifican una función, una clase o un componente.

- ⚪ **de integración**: Pruebas de caja blanca que verifican que varios componentes funcionan bien juntos.

- ✔️ **de inicio a fin**: Pruebas de caja negra que replican el comportamiento de un usuario ante un sistema completo.

> Otras: de regresión, de humo, de aceptación...

### ⌚ Después -> Durante -> Antes

- ❌ **Después** o mucho después _legacy_. Es costoso, pero imprescindible para un _refactoring_ y muy habitual en un _end to end_

- ⚪ **Durante** es aburrido pero necesario para las pruebas de integración.

- ✔️ **Antes** El conocido como _TDD_ para pruebas unitarias o _BDD_ para las de integración. Menos costoso, más divertido y con mucho mejor diseño resultante.

## 👨‍🎓 Qué hay que saber para programar tests.

### 1️⃣ Mantra

- **El código de prueba no es como el código de producción:** diséñalo para que sea simple, corto, sin abstracciones, agradable de leer. Uno debe mirar una prueba y obtener la intención al instante.

### 2️⃣ Siglas y conceptos

- **SUT**: _System (Subject) Under Test_. Lo que se está probando.

- **DOCs**: _Depended On Components_. Lo que se necesita para que funcione el SUT.

### 3️⃣ Secciones: Arrange, Act & Assert (AAA Pattern)

- **Arrange**: Prepara y organiza lo que necesitas.

- **Act**: Ejecuta el código y obtén una respuesta.

- **Assert**: Verifica que la respuesta es la esperada.

### 4️⃣ Cuestiones: Given, Should, Actual, Expected.

- **Given**: 📃 Texto. Condiciones de la prueba. _(Arrange)_

- **Should**: 📃 Texto. Funcionalidad esperada.

- **Actual**: 🎰 Variable. El resultado obtenido. _(Act)_

- **Expected**: 💰 Variable. La respuesta esperada. _(Assert)_

### 5️⃣ Test Doubles: Simuladores para no depender de las dependencias DOC.

- **Dummy**: Datos requeridos para que el SUT funcione, pero que no se usan durante la prueba. _(Carga previa de una base de datos)_

- **Stub**: Un objeto que cumpliendo una interfaz de un DOC tiene una respuesta constante y predeterminada. _(Responder como lo haría un llamada http)_

- **Fake**: Un objeto que realiza una funcionalidad coherente pero simplificada de un DOC. _(Simular una base de datos en memoria)_

- **Spy**: Cuenta las llamadas a una función o método. _(Comprobar que se ejecuta una acción un determinado número de veces)_

- **Mock**: Monitoriza el uso de un objeto y las llamadas a una función junto con sus argumentos. _(Simular un envío de correo completo)_

### 6️⃣ Comprobaciones: igualdad, existencia, comparación, pertenencia, excepciones y negación

- **igualdad**: El valor actual es igual al esperado.

- **existencia**: El valor actual existe.

- **comparación**: El valor actual es mayor o menor que el esperado.

- **pertenencia**: El valor actual contiene o está contenido en el esperado.

- **excepciones**: Se espera que una excepción sea lanzada.

- **negación**: Niega cualquiera de los anteriores.

### 7️⃣ Consejos generales

- **incorpora herramientas**: Puedes empezar de cero, pero hay muchas ayudas.

- **evita arreglos globales**: Cada prueba deber ser autónoma e independiente.

- **datos realistas en los fakes**: Nada de _foo_ _bar_ _baz_ _asdf_

- **usa etiquetas o códigos**: Útil para buscar resultados o pre filtrar pruebas.

- **public black box**: Prueba los métodos públicos.

- **evita los mocks**: Mejor usa _Stubs_ y _Spies_.

- **haz alguna prueba**: Esto no va de todo o nada.

## 🛠 Herramientas

- Utilidades para probar aplicaciones desarrolladas con tecnología web.

### Puppeteer

[Puppeteer](https://pptr.dev/) es excelente para manipular y simular cualquier actividad con el navegador ideal para _e2e_ no funcional.

### Cypress

[Cypress](https://www.cypress.io/) es un framework de pruebas funcionales de integración o _e2e_. Se ejecuta en el navegador independiente del código bajo prueba.

### Jest

[JEST](https://jestjs.io/) es un framework muy popular porque requiere _zero configuration_. Es muy ligero y sencillo. Ideal para _unit testing_ y _TDD_.

### Otros

- **[Playwright](https://github.com/microsoft/playwright)** automatizador de diversos navegadores al estilo Puppeteer.

- **[Karma](https://karma-runner.github.io/latest/index.html)** es un ejecutador de pruebas muy interesante para integración continua.

- **[Jasmine](https://jasmine.github.io/)** muy completo y bueno para user-behavior por su expresividad

- **[Mocha](https://mochajs.org/)** muy utilizado para NodeJS.

- **[Chai](https://www.chaijs.com/)** librería muy adecuada para BDD con NodeJS.
