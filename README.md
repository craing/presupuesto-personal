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

## Tus datos y seguridad

- Todo se guarda en el `localStorage` de tu navegador. El código publicado es público, pero **tus cifras nunca se suben** a ningún lado.
- La página incluye una política de seguridad (CSP) que **bloquea toda conexión de red** y cualquier recurso externo, así que la app no puede enviar datos fuera de tu dispositivo.
- **Respaldos cifrados:** "Exportar respaldo" pide una contraseña y cifra el archivo con AES-256-GCM (clave derivada con PBKDF2-SHA256, 600.000 iteraciones). Al importarlo se pide la misma contraseña. **Si la olvidas, el respaldo no se puede recuperar.** Existe la opción de exportar sin cifrar, no recomendada.
- Cada navegador o dispositivo tiene sus propios datos: para pasarlos de uno a otro, exporta el respaldo en uno e impórtalo en el otro.
- Recomendaciones: bloqueo con PIN/biometría en tus dispositivos, verificación en dos pasos (2FA) en GitHub y no compartir respaldos por chat o correo.
