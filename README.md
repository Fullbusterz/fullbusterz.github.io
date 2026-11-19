# fullbusterz.github.io

Solo sirve `/.well-known/assetlinks.json`: le dice a Android que la APK **Ruta** (`com.flixescola.ruta`,
firmada con la clave cuya huella SHA-256 está en ese archivo) es la dueña de
https://fullbusterz.github.io/EasyEscolaVins/. Con eso la APK abre la app a pantalla completa, sin barra del
navegador, y el botón «Traer la ruta del portal» no pregunta.

- `.nojekyll` hace falta: sin él GitHub Pages no publica carpetas que empiezan por punto (`.well-known`).
- Si se cambia la clave de firma de la APK, hay que cambiar aquí la huella.
- La app vive en su propio repositorio (`Fullbusterz/EasyEscolaVins`); este no la toca.
