# Gestor de Pedidos — Bolsas Fantasía

Aplicación web desarrollada para gestionar y generar pedidos de bolsas ecológicas personalizadas. Surgió como solución a una necesidad operativa real: reemplazar el proceso manual de carga de pedidos por una herramienta digital que genera un resumen estructurado listo para usar.

🔗 **Demo en vivo:** [tweegio.github.io/carga_de_pedidios_TXT](https://tweegio.github.io/carga_de_pedidios_TXT/)

---

## Vista previa

![Gestor de Pedidos Preview](logo_txt.png)

---

## ¿Qué problema resuelve?

El proceso de toma de pedidos para bolsas personalizadas, requería registrar múltiples variables por producto: modelo, medida, color y cantidad. Hacerlo manualmente generaba errores y pérdida de tiempo. Esta app centraliza la carga, valida los datos y genera un resumen del pedido exportable en formato TXT, listo para enviar o preparación de pedidos de los vendedores externos de la empresa.

---

## Tecnologías utilizadas

- HTML5
- CSS3 — diseño responsivo
- JavaScript vanilla — lógica de formulario, validaciones, generación dinámica del resumen y exportación TXT

---

## Funcionalidades

- Selección de **fecha de entrega**
- Campos de **nombre de cliente** y **número de orden**
- Selector de **modelo de bolsa** con más de 25 variantes (medidas y diseños)
- Selector de **color** (9 opciones)
- Campo de **cantidad**
- Botón **Agregar Producto** — agrega líneas al resumen sin recargar la página
- **Resumen del pedido** generado dinámicamente en tiempo real
- **Confirmar Pedido** — genera y descarga el archivo `.txt` con todos los datos estructurados
- **Borrar Pedido** — limpia el formulario y el resumen completo
- Campo de **comentarios adicionales**
- Página de **indicaciones de uso** para onboarding de nuevos usuarios

---

## Modelos de bolsa disponibles

**Por medida (Riñón):** 22.5x30 · 30x30 · 30x40 · 38x40 · 45x40

**Por medida (Manija):** 30x30 · 38x40 · 45x40 · 50x60

**Diseños especiales:** Great Rosa · Gatitos · Rock Nacional · Maradona · Cat · Gato Chino · Mandala · Vincent · Gafas · Fly · Guau Grande · Positive · Navidad · Año Nuevo · Pinoel

---

## Estructura del proyecto

```
/
├── index.html
├── indicaciones_de_uso.html
├── logo_txt.png
├── css/
│   └── styles.css
└── js/
    └── script.js
```

---

## Decisiones técnicas

**Generación de TXT del lado del cliente.** La exportación del pedido se resuelve completamente en el navegador usando la API `Blob` y un link de descarga dinámico, sin necesidad de servidor ni backend. Esto permite que la app funcione offline y sea deployable como sitio estático.

**Proyecto nacido de una necesidad real.** La app fue desarrollada a partir de la experiencia directa en gestión de pedidos en TXT Transporte y Logística, lo que permitió diseñar el flujo de datos y la interfaz con conocimiento real del proceso operativo.

**Sin dependencias externas.** Todo el comportamiento está implementado en JavaScript vanilla para mantener el proyecto liviano y sin overhead de librerías.

---

## Cómo correrlo localmente

```bash
git clone https://github.com/tweegio/carga_de_pedidios_TXT.git
cd carga_de_pedidios_TXT
# Abrí index.html en tu navegador o usá Live Server en VS Code
```

No requiere instalación de dependencias ni build process.

---

## Autor

**Sergio Pereira** — Desarrollador Front-End & Técnico Informático

- 🌐 [Portfolio](https://tweegio.github.io/portfolio)
- 💼 [LinkedIn](https://www.linkedin.com/in/sergio-pereira-development/)
- 🐙 [GitHub](https://github.com/tweegio)

---

*© 2024 Tweegio*
