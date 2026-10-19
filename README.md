# Presupuesto Personal

App web de presupuesto personal en español (Chile), en un solo archivo `index.html`. No requiere servidor, instalación ni conexión a internet.

## Cómo usarla

1. Descarga o clona el repositorio.
2. Abre `index.html` en tu navegador (doble clic). En el celular puedes publicarla con GitHub Pages y agregarla a la pantalla de inicio.

## Funciones

- **Resumen:** ingresos, gastos y saldo del mes, gráfico de gastos por categoría, avance del presupuesto, fondo de emergencia y deudas.
- **Movimientos:** registra ingresos y gastos (fecha, tipo, monto, categoría y nota). Edita (✏️) o borra (🗑️). Filtra por tipo, categoría o texto.
- **Presupuesto:** monto mensual por categoría (aplica a todos los meses). Barra verde (<80 %), amarilla (80–100 %) o roja (>100 %).
- **Fondo de emergencia:** define una meta en CLP y registra aportes o retiros; muestra el % de avance y cuántos meses de gasto cubre.
- **Deudas:** nombre, saldo, cuota mensual y tasa (% mensual). Muestra el total adeudado y el orden de pago sugerido:
  - *Avalancha:* primero la de mayor tasa (pagas menos intereses).
  - *Bola de nieve:* primero la de menor saldo (victorias rápidas).
- **Selector de mes** (arriba): ◀ ▶ o elige un mes para ver el historial.
- **Categorías y datos:** agrega, renombra, cambia color o borra categorías (los movimientos se reasignan). Exporta/importa respaldo JSON y exporta movimientos a CSV (separador `;`, se abre directo en Excel).
- **Tema:** botón 🌓 alterna automático / claro / oscuro.

## Tus datos

Todo se guarda en el `localStorage` de tu navegador: nada sale de tu equipo. Si borras los datos del navegador o cambias de dispositivo, se pierden, así que **exporta un respaldo JSON periódicamente** e impórtalo en el otro equipo.
