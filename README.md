# Giros de presupuestos máximos · Dashboard

Dashboard interactivo (diseño Edelman) a partir del consolidado de giros de presupuestos máximos (Art. 240 Ley 1955 de 2019).

Pestañas: Concepto de pago · EPS · Giro directo a IPS · Percepción en salud.
Filtros: año y mes de pago, concepto (periodo de asignación), EPS y régimen.

## Contenido

- `index.html`: el dashboard completo en un solo archivo (datos, fuentes, logos y estilos incluidos).

## Publicar en GitHub Pages

1. Sube `index.html` y este `README.md` a la raíz del repositorio.
2. En el repositorio: **Settings → Pages**.
3. En *Source* elige **Deploy from a branch**, rama `main`, carpeta `/ (root)` y guarda.
4. En uno o dos minutos el tablero queda en `https://<usuario>.github.io/<repositorio>/`.

## Actualizar los datos

- **Rápido (cada usuario):** botón **Cargar Excel actualizado** en el encabezado. Lee las hojas `BBDD Giros a EPS`, `BBDD Giros a IPS` y `Encuestas de percepción en salud`. Los datos se quedan solo en ese navegador; **Restaurar datos originales** vuelve a los del archivo.
- **Para todos:** hay que generar un `index.html` nuevo con el Excel actualizado y reemplazarlo en el repositorio.

## Notas

- La carga de Excel necesita conexión a internet (usa la librería SheetJS desde su CDN). El resto funciona sin conexión.
- `index.html` cuenta con una ventana de ingreso con contraseña (`EdelmanCOLOMBIA`) para restringir el acceso al tablero y proteger la visualización de los datos.
