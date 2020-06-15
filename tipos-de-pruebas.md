---
marp: true
---

# 🔀 Tipos de Pruebas

Hay una prueba para cada situación.

---

> _"Escribe tests. No demasiados. Principalmente de integración."_
>
> ✍🏼 Kent C. Dodds

---

### 🤖 Manuales -> Programadas

- ❌ Dependemos de las personas

- ✅ Se pueden configurar y lanzar automáticamente

---

### ⚖ Técnicas -> Funcionales

- ⚪ Se puede comprobar el rendimiento, la seguridad, usabilidad...

- ✅ La función del software, su utilidad.

---

### 🔎 Unitarias -> De integración -> De inicio a fin

- ✅ **unitarias**: Caja blanca. Verifican una función, una clase o un componente.

- ✅ **de integración**: Caja blanca. Verifican que varios componentes funcionan juntos.

- ✅ **de inicio a fin**: Caja negra. Replican comportamiento de usuario en sistema.

> Otras: de regresión, de humo, de aceptación...

---

### ⌚ Después -> Durante -> Antes

- ✅ **Después** Costoso, pero imprescindible para un _refactoring_ y _end to end_

- ✅ **Durante** Aburrido pero necesario para las pruebas de integración.

- ✅ **Antes**  _TDD_ para pruebas unitarias o _BDD_ para las de integración.

  - Menos costoso,
  - Más divertido
  - y con mucho mejor diseño resultante.
