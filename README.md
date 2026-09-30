# Costeo de Tortas — app Android

Calculadora de costo y precio sugerido de tortas y cupcakes (Colores · Tortas Decoradas).

- `www/` → la calculadora. Se publica en GitHub Pages: https://luis19842021.github.io/costeo-tortas-app/
- La app Android abre esa página, así que **se actualiza sola** con cada `git push` que cambie `www/`.
- `.github/workflows/pages.yml` → publica la web.
- `.github/workflows/build-apk.yml` → arma el APK (solo cuando cambia la configuración de la app, o a mano desde Actions → "Compilar APK" → Run workflow).

## Actualizar la calculadora
```bash
git add .
git commit -m "Qué cambié"
git push
```
En un par de minutos la app del celular muestra la versión nueva (cerrala y abrila de nuevo).

## Instalar el APK
Actions → "Compilar APK" (tilde verde) → Artifacts → `costeo-tortas-apk` → pasar `app-debug.apk` al celular e instalar.

Los precios que cambies en la app se guardan en el celular. Después de la primera carga, la app también abre sin internet.
