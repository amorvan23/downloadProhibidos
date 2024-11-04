# Guía de Instalación y Uso del Sistema

## Paso 1: Descargar e Instalar Python

1. Verificar si ya tienes Python instalado:
- Abre el Símbolo del sistema en Windows (busca 'cmd' en el menú de inicio).
- Escribe el siguiente comando y presiona Enter:
    python --version
- Si tienes Python instalado, verás la versión instalada (por ejemplo, 'Python 3.10.0'). Si no tienes Python instalado, el sistema te indicará que el comando no se reconoce.

2. Instalar Python (si no está instalado):
- Abre tu navegador y ve a la página oficial de Python en https://www.python.org/downloads/.
- Descarga la versión recomendada para tu sistema operativo.
- Abre el archivo descargado para iniciar el instalador.
- Importante: Asegúrate de marcar la casilla que dice 'Add Python to PATH' (Agregar Python al PATH).
- Haz clic en 'Install Now' y espera a que la instalación termine.
- Una vez completada, vuelve a verificar la instalación repitiendo el primer paso de este tutorial.

## Paso 2: Descargar el proyecto e Instalar las Dependencias Necesarias

Link de descarga del proyecto: https://drive.google.com/file/d/1MKFOEbfTsUgb1GxMTB712nK3v2UZVAhm/view?usp=sharing

- Descomprimir Zip descargado y situarlo en el lugar deseado (Depende del sitio donde se situe, el sistema necesitará permisos de administrador para descargar ficheros de forma automática)

Para que el sistema funcione correctamente, necesitarás instalar ciertas bibliotecas de Python. Esto se puede hacer de dos maneras:

Opción A: Instalar dependencias manualmente mediante PIP
1. Abre el Símbolo del sistema (cmd) en Windows.
2. Navega hasta el directorio donde tienes los archivos del proyecto.
3. Escribe el siguiente comando para instalar las dependencias necesarias:
    pip install -r requirements.txt

Opción B: Instalar dependencias automáticamente con el archivo instalar_dependencias.bat
1. Haz doble clic en el archivo instalar_dependencias.bat.
2. Este archivo ejecutará automáticamente el proceso para instalar las dependencias usando PIP.

## Paso 3: Ejecutar el archivo ejecutar_prohibidos.bat (Primera Ejecución)

1. Haz doble clic en el archivo ejecutar_prohibidos.bat para ejecutar el sistema por primera vez.
2. En esta primera ejecución, el sistema creará una estructura de archivos y carpetas necesaria.
3. Entre los archivos creados, verás uno llamado config.json en el directorio del proyecto.

## Paso 4: Configurar el archivo config.json

1. Abre el archivo config.json utilizando un editor de texto simple, como el Bloc de notas.
2. Dentro de este archivo encontrarás diversas configuraciones que puedes ajustar según tus requisitos.
3. Guarda el archivo después de realizar los cambios.

## Paso 5: Copiar el archivo private_key (clave privada)

1. Es necesario tener una clave privada (private_key) obtenida al solicitar acceso a la Consellería.
2. Si usas el software certi_generator, la clave privada estará en el archivo .zip que descargaste.
3. Copia este archivo private_key en el directorio key en la estructura creada

## Paso 6: Segunda Ejecución del archivo ejecutar_prohibidos.bat

1. Con el config.json configurado y la clave privada en la carpeta key, ejecuta ejecutar_prohibidos.bat de nuevo.
2. En esta segunda ejecución, el sistema descargará un archivo en la carpeta descargas.
3. La carpeta descarga_actual se actualizará, conteniendo solo el archivo más reciente descargado.

## IMPORTANTE
### El sistema gestiona unos contadores con identificadores y un sistema de Logging. Es importante no eliminar ficheros de los que se generan automáticamente, ya que si se elimina el fichero db o alguno de los ficheros necesarios, el sistema puede presentar incosnsisténcias



