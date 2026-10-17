# MiTube Downloader — proyecto Android inicial

## Estado real de esta versión
Este proyecto es una **base funcional de interfaz y descarga directa**, no una aplicación completa para descargar desde páginas de YouTube.

Incluye:
- Interfaz nativa Android en español.
- Selector MP4/MP3.
- Descarga mediante el gestor de descargas de Android de enlaces HTTPS directos a archivos `.mp4` o `.mp3`.
- Aviso de descarga y guardado en `Descargas`.

No incluye todavía:
- Resolución de enlaces `youtube.com` / `youtu.be`.
- Extracción de audio MP3 desde un vídeo MP4.
- Selección de calidad adaptativa de YouTube.
- Compilación ni firma de una APK.

La limitación es deliberada: el enlace de una página de YouTube no es un enlace directo al archivo multimedia. Para vídeos propios, una vía compatible es descargarlos desde YouTube Studio y luego usar el archivo local; para otras fuentes, utiliza enlaces de descarga autorizados.

## Cómo abrir y compilar
1. Instala Android Studio desde el sitio oficial de Android Developers.
2. Descomprime este ZIP.
3. En Android Studio, selecciona **Open** y elige la carpeta `MiTubeDownloader-Android`.
4. Espera a que Gradle termine de sincronizar.
5. Conecta tu Android con la depuración USB activada o usa un emulador.
6. Pulsa **Run** para probar la aplicación.
7. Para crear una APK de prueba: **Build > Build APK(s)**. Android Studio mostrará la ruta del archivo generado.

## Requisitos
- Android Studio con JDK integrado.
- SDK de Android 35 instalado.
- Conexión a Internet para descargar dependencias de Gradle.

## Próximo desarrollo necesario para cumplir el objetivo completo
Hace falta incorporar un componente de procesamiento de medios que pueda operar legalmente sobre los archivos o fuentes autorizadas, implementar la extracción/conversión a MP3 y probar el manejo de formatos y errores. Este ZIP no debe presentarse como si ya realizara esas funciones.
