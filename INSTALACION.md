# Instalación portable en Windows

## Primera ejecución

1. Abre https://github.com/pedroarce/antenna-pattern/releases/latest .
2. En **Assets**, descarga el ZIP que termina en **Windows-x64.zip**.
3. Haz clic derecho en el archivo descargado y elige **Extraer todo**.
4. Guarda la carpeta `AntennaPattern` en una ubicación donde puedas escribir.
5. Ejecuta `AntennaPattern.exe`. Puedes crear un acceso directo en el Escritorio.

No necesitas instalar Python. Mantén `_internal` y todas sus subcarpetas junto
al `.exe`. No confundas el texto de patrones MSI con un instalador de Windows:
la salida de patrones de esta app utiliza `.txt`.

El ejecutable no está firmado digitalmente. Si Windows muestra un aviso,
comprueba la procedencia y el SHA-256 antes de decidir si ejecutarlo; no es
necesario desactivar el antivirus ni otras protecciones.

## Comprobar la descarga

Descarga también `SHA256SUMS.txt`. En PowerShell, dentro de la carpeta de descarga:

```powershell
Get-FileHash -LiteralPath .\AntennaPattern-0.20.0-Windows-x64.zip -Algorithm SHA256
```

Compara el resultado con el valor del ZIP en `SHA256SUMS.txt`.

## Tu trabajo y las claves de IA

Guarda tus proyectos `.antproj` fuera de la carpeta de la aplicación. Las claves
de IA se configuran en Ayuda y pertenecen a cada usuario de Windows; no vienen
incluidas en la descarga. La edición local, OpenCV y los gráficos no requieren IA.

Para mover un proyecto digitalizado a otra PC basta su `.antproj`, que incorpora
las imágenes. Conserva aparte los archivos originales que necesites archivar.

## Actualizar o retirar

Guarda y cierra la app. Extrae la versión nueva en otra carpeta, abre allí el
ejecutable y carga tus proyectos. Conserva la versión anterior hasta comprobar
tu trabajo. Para retirar la versión portable, elimina su carpeta una vez que
hayas guardado los proyectos en otra ubicación.

## Si algo falla

- Si falta una DLL, vuelve a extraer el ZIP completo y conserva `_internal`.
- Si el archivo de patrón no abre, copia el mensaje y comprueba si es MSI/TXT o NSMA.
- Si falla la IA, revisa proveedor, modelo, cuota y clave sin publicarla.
- Usa **Ayuda → Manual de usuario (PDF)** para los procedimientos completos.

Plataforma preparada: Windows x64. No hay paquete nativo para macOS o Linux.

