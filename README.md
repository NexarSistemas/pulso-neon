# ⚡ Pulso Neón

Juego arcade de reflejos, precisión y concentración con estética neón. Desarrollado en **HTML, CSS y JavaScript puro**, sin frameworks, cuentas ni servidor.

**Versión actual: v1.5.2** · Desarrollado por **Nexar Sistemas**.

## Cómo se juega

1. Tocá **EMPEZAR**.
2. Cuando la aguja llegue a la zona de acierto, presioná **PULSAR**.
3. Acertá para avanzar. Si fallás o completás dos vueltas sin pulsar, perdés.
4. Superá el **nivel 29 con un acierto válido** para ganar la partida.

## Dificultad

- **Niveles 1–9:** objetivo fijo y velocidad progresiva.
- **Niveles 10–19:** cambios inesperados de dirección y cambio de estética.
- **Niveles 20–29:** también gira la zona de acierto, más lentamente y en sentido contrario.
- **Victoria:** solo al acertar el nivel 29; llegar al nivel no es suficiente.

## Características

- Controles táctiles y respuesta al contacto inicial del dedo.
- Efectos sonoros con opción de silencio.
- Récord y estadísticas almacenados en el navegador.
- Pantalla de victoria al completar el desafío.
- PWA preparada para instalar y usar sin conexión, una vez publicada mediante HTTPS.

## Jugar localmente

Para probar la jugabilidad podés abrir `index.html` directamente. Para probar la PWA y el Service Worker, usá un servidor local:

```bash
python3 -m http.server 8000
```

Abrí `http://localhost:8000`. La instalación PWA requiere **HTTPS o localhost**, no funciona con `file://`.

## Publicación en GitHub Pages

En **Settings → Pages**, seleccioná **Deploy from a branch**, rama `main`, carpeta `/ (root)` y guardá.

Una vez activado GitHub Pages, la dirección prevista del juego es:

https://nexarsistemas.github.io/pulso-neon/

Desde Chrome en Android se puede utilizar la opción **Instalar aplicación** cuando esté disponible. La PWA guarda recursos para permitir jugar sin conexión después de la primera carga correcta.

## Privacidad

Los récords y las estadísticas se guardan **solo en este dispositivo**, usando almacenamiento local del navegador. No hay cuentas ni sincronización. Borrar los datos del sitio elimina esos registros.

## Versionado

Se usa el formato **SemVer** (`MAJOR.MINOR.PATCH`), con mensajes de commit en español, historial en [CHANGELOG.md](CHANGELOG.md) y versión actual en [VERSION](VERSION).

La versión visible en el juego, `VERSION` y la etiqueta de cada lanzamiento deben coincidir. Los tags y las releases se crean únicamente después de validar la versión correspondiente.

## Estado

**v1.5.2 — juego completo y PWA preparada.** Falta activar GitHub Pages y verificar instalación y funcionamiento sin conexión en Android. No se prevén nuevas mecánicas por ahora.
