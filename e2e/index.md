---
marp: true
---

# E2E Pruebas externas de principio a fin
##   Puppeteer para comprobación de existencia, navegación, tamaño, velocidad y otras métricas.

> _"Si un usuario final percibe una mal rendimiento en tu website, su siguiente click probablemente sea en tu-competencia.com"_
>
> -- ✍️ **Ian Molyneaux**

---

## Lo primero es **software que funcione**.

Y cuando hablamos de una _web_ la primera garantía debe ser la **existencia y la descarga rápida** de contenido relevante.

---

- Propongo utilizar es [Puppeteer](https://pptr.dev/).
- Aunque se puede con [Cypress](https://www.cypress.io/) o [Playwright](https://github.com/microsoft/playwright).

---

## **Objetivos** de la prueba:

- ✅ Garantizar que una ruta existe.

- ✅ Comprobar que el contenido es el esperado.

- ✅ Validar que sus métricas entran en un rango esperado.

---

🔥 Casi [pruebas de humo](https://es.wikipedia.org/wiki/Pruebas_de_humo)

- Simple
- Asequible
- Recomendable

