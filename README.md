# Procesador de Archivos CSV y Excel con Flask
## Descripción
Esta aplicación web, construida con Flask, permite cargar archivos CSV y procesarlos en diferentes formatos de salida. Dependiendo del tipo de archivo seleccionado, se realizan transformaciones y se devuelven archivos Excel o CSV modificados con una estructura y formato específicos.

## Características
Tipos de Procesamiento: Soporta cuatro tipos de procesamiento (1, 2, 3 y 4) que aplican diferentes modificaciones y formatos a los datos.

Procesamiento en memoria: Los archivos se procesan directamente en memoria sin necesidad de guardarlos en el servidor.

Interfaz sencilla: Carga de archivos a través de una página web y descarga directa del archivo procesado.
## Requisitos

- Python 3.11.4
- Librerías requeridas:
  - Flask
  - pandas
  - openpyxl

## Instalación
Clonar este repositorio.

```
git clone https://github.com/alejomazov/file_change.git
cd file_change
```
Instalar las dependencias con pip:

```
pip install -r requirements.txt
```
Ejecutar la aplicación:
```
python app.py
```
Abrir tu navegador y dirigirte a http://127.0.0.1:5000/.

## Uso
1. Dirígete a la página principal.
2. Selecciona el archivo CSV que deseas procesar.
3. Elige el tipo de procesamiento según las modificaciones que necesites aplicar:
   - Tipo 1: Reorganiza y modifica columnas específicas.
   - Tipo 2: Reorganiza columnas, extrae grupos y ordena según criterios específicos.
   - Tipo 3: Renombra columnas y genera un archivo CSV compatible con "Tangram".
   - Tipo 4: Realiza modificaciones similares al tipo 3, pero con un tipo diferente.
4. Introduce un nombre de descarga para el archivo resultante.
5. Haz clic en "Subir" y espera la descarga del archivo procesado.
## Estructura del Proyecto
bash
Copiar código
```
/procesador-csv-flask
│
├── app.py                 # Código principal de la aplicación Flask
├── templates/
│   └── upload.html        # Plantilla HTML para la interfaz de usuario
├── README.md              # Documentación del proyecto
├── vercel.json            # 
└── requirements.txt       # Dependencias del proyecto

```
## Personalización
Si necesitas realizar ajustes en la lógica de procesamiento, puedes editar las funciones procesar_tipo_1, procesar_tipo_2, procesar_tipo_3 o procesar_tipo_4 dentro del archivo app.py.

## Contribuciones
Las contribuciones son bienvenidas. Si tienes alguna idea para mejorar la aplicación o encuentras algún error, por favor crea un issue o un pull request.
