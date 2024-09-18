# fillmypdf
Aplicación para rellenar formularios PDF de manera eficiente, permitiendo a los usuarios cargar documentos, visualizar y completar campos repetitivos. Próximamente, incluirá OCR para extraer datos automáticamente y optimizar el proceso.
### Resumen de la Aplicación
Objetivo de la Aplicación: La aplicación es un rellenador de formularios PDF que facilita el proceso de completar documentos repetitivos, como formularios de cliente o de cuenta, que suelen solicitar los mismos datos (nombre, número de documento, etc.). La idea es que los usuarios puedan cargar un documento, visualizarlo, y luego rellenar formularios asociados de manera eficiente. En el futuro, la aplicación incluirá una funcionalidad de OCR para extraer automáticamente datos del documento y pre-rellenar los formularios, ahorrando aún más tiempo.

### Estructura Principal:

App Component:

Contiene dos columnas:
Documentos: Maneja la carga y visualización de los documentos.
Formularios: Permite al usuario seleccionar y rellenar formularios específicos basados en los documentos cargados.
Gestiona la selección y eliminación de archivos PDF y la asociación de estos archivos con tipos de formularios.
FileSelector Component:

Permite al usuario seleccionar archivos PDF desde su dispositivo.
Verifica si el PDF seleccionado tiene campos rellenables antes de permitir que sea agregado a la lista de documentos.
PDFViewer Component:

Carga y muestra el documento PDF.
Renderiza los campos de formulario asociados con el tipo de formulario seleccionado.
Permite al usuario rellenar estos campos manualmente.
Guarda el PDF con los campos rellenados y permite visualizarlo.
DocumentList Component:

Lista los documentos disponibles (aunque por ahora es estático) en la columna de documentos.
Configuración del Formulario:

formConfig.json:
Define los campos de formulario para diferentes tipos de documentos (ejemplo: cliente).
Cada tipo de documento tiene campos específicos, como nombre, fecha de nacimiento, número de CI, y celular.

### Futuras Mejoras:

OCR: Extraer automáticamente los datos de los documentos y pre-rellenar los campos de formularios, permitiendo correcciones manuales si es necesario.
Expansión de Formatos: Aceptar y procesar otros formatos de documentos además de PDF.
Mejoras en la Interfaz: Hacer que la selección de tipos de formularios sea más intuitiva, posiblemente inferida directamente del documento cargado.
