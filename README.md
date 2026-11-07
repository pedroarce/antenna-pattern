# Antenna Pattern

Editor de patrones de radiación de antenas para **Windows x64**.

**[Descargar la última versión](https://github.com/pedroarce/antenna-pattern/releases/latest)** · **[Manual de usuario PDF](https://github.com/pedroarce/antenna-pattern/releases/download/v0.20.0/Manual_de_usuario.pdf)** · **[Cómo instalar](INSTALACION.md)**

## Descargar y ejecutar

1. Abre **Releases** y descarga `AntennaPattern-0.20.0-Windows-x64.zip` en **Assets**.
2. Haz clic derecho sobre el ZIP y selecciona **Extraer todo**.
3. Abre la carpeta extraída `AntennaPattern` y ejecuta **AntennaPattern.exe**.

Es una aplicación portable: no necesita instalar Python ni un asistente de
instalación. Conserva la carpeta `_internal` junto al ejecutable. No ejecutes
el programa dentro del ZIP ni copies únicamente el `.exe`.

Los enlaces **Source code (zip/tar.gz)** que añade GitHub contienen la
documentación de este repositorio; para usar la app descarga el ZIP de Windows.

## Funciones

- Importación, edición y exportación de patrones MSI en texto `.txt`.
- Lectura y edición NSMA con frecuencias, polarizaciones, cortes y fase.
- Gráficas polares y cartesianas con zoom e historial de vistas.
- Creación de patrones desde cero y modelos de referencia UIT-R.
- Digitalización manual y seguimiento de curvas mediante OpenCV.
- Extracción de tablas H/V con Gemini u OpenAI, para revisión posterior.
- Tablas 3D, visualización, extracción H/V y análisis de directividad.
- Envolventes de ganancia absoluta, proyecto editable y exportación de imágenes.

La IA es opcional y requiere una clave propia del proveedor. Puede generar
costos según la cuenta y modelo elegidos. Los resultados extraídos de imágenes
son aproximaciones que deben revisarse. La directividad necesita datos 3D
esféricos completos; la representación desde dos cortes H/V es ilustrativa.

## Manual y ayuda

El PDF de 55 páginas está disponible en Releases y dentro de la descarga.
También se abre desde **Ayuda → Manual de usuario (PDF)**.

Para reportar errores, abre un [Issue](https://github.com/pedroarce/antenna-pattern/issues)
con versión, pasos para reproducir y mensaje de error. No publiques claves API
ni archivos confidenciales. Incluye muestras solo si puedes compartirlas.

## Distribución

Este repositorio publica las descargas y documentación. Las dependencias
conservan sus licencias y avisos dentro del paquete. La versión 0.20.0 se ha
comprobado mediante autoprueba del ejecutable; la prueba en un Windows limpio
sigue pendiente. El ejecutable todavía no tiene firma digital.

