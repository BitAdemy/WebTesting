---
marp: true
---

# 👨🏼‍🏫 Filosofía y patrones

Qué hay que saber para programar tests.

---

### 1️⃣ Mantra

- **El código de prueba no es como el código de producción.**

- Simple, corto, sin abstracciones, fácil de entender.

---

### 2️⃣ Siglas y conceptos

- **SUT**: _System (Subject) Under Test_.

- **DOCs**: _Depended On Components_.

---

### 3️⃣ Secciones: Arrange, Act & Assert (AAA Pattern)

- **Arrange**: Prepara y organiza lo que necesitas.

- **Act**: Ejecuta el código y obtén una respuesta.

- **Assert**: Verifica que la respuesta es la esperada.

---

### 4️⃣ Cuestiones: Given, Should, Actual, Expected.

- **Given**: 📃 Texto. Condiciones de la prueba.

- **Should**: 📃 Texto. Funcionalidad esperada.

- **Actual**: 🎰 Variable. El resultado obtenido.

- **Expected**: 💰 Variable. La respuesta esperada.

---

### 5️⃣ Test Doubles: Simuladores para no depender de las dependencias.

- **Dummy**: _(Carga previa de una base de datos)_

- **Stub**: _(Responder como lo haría un llamada http)_

- **Fake**: _(Simular una base de datos en memoria)_

- **Spy**: _(Comprobar llamadas a funciones)_

- **Mock**: _(Simular un envío de correo completo)_

---

### 6️⃣ Comprobaciones:

- **igualdad**

- **existencia**

- **comparación**

- **pertenencia**

- **excepciones**

- **negación**

---

### 7️⃣ Consejos generales

- **incorpora herramientas**

- **evita arreglos globales**

- **datos realistas en los fakes**

- **usa etiquetas o códigos**

- **public black box**

- **evita los mocks**

- **haz alguna prueba**
