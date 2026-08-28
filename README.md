# TaiChi Vital — App

App post-compra de TaiChi Vital: entrenamientos (Tai Chi, Yoga en Silla, Pilates, Micro Workouts),
comidas, seguimiento de progreso e imprimibles. Inspirada en la estructura real de la app de
SoonBody (soonbody.com/app), con contenido, programas y marca propios.

## Estructura
- `index.html` — la app completa (motor vanilla JS, sin frameworks, 1 solo archivo).
- `server.js` — servidor estático minimalista para producción / Railway.
- `images/` — fotos de los programas.

## Cómo funciona
No hay backend todavía: **todo el registro (agua, calorías, peso, ánimo, racha, entrenamientos
completados) se guarda en `localStorage` del propio dispositivo**, por eso no hay login real y
cada navegador/celular tiene su propio progreso independiente.

## Pendiente para que sea un producto real
- **Cuentas de usuario reales** (login, sincronización entre dispositivos) — necesita backend +
  base de datos.
- **Checkout real**: el banner "Suscribite" es un placeholder, no cobra nada todavía.
- **Videos de los ejercicios**: hoy cada ejercicio es una tarjeta con nombre/duración/series, sin
  video ni imagen del movimiento.
- **Imprimibles reales**: las guías están bloqueadas con un candado de ejemplo; no hay PDFs de
  verdad generados todavía.
- **Recetas/registro de comidas real**: hoy "Registrar alimento" solo suma un valor de ejemplo.

## Correr en local
```bash
npm start
```
Abrí `http://localhost:3000`.

## Deploy en Railway
Igual que el quiz: **New Project → Deploy from GitHub repo** → elegí este repositorio. Railway
detecta Node automáticamente y corre `npm start`.
