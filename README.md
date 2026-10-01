# Sistema CRUD - Gestor de Personas

## Integrantes

- Gabriel Plata - 01240372047
- Valery Montes - 01240372023

## Descripción

Este proyecto consiste en un sistema CRUD desarrollado en Python utilizando Gradio.

El sistema permite gestionar registros de personas mediante una interfaz gráfica sencilla. Los registros se almacenan temporalmente en una lista y pueden ser agregados, consultados, editados o eliminados.

También permite exportar los registros almacenados a un archivo CSV.

## Funcionalidades

El sistema cuenta con las siguientes operaciones:

- **Agregar persona:** permite registrar una persona ingresando nombre, apellido, edad y ciudad.
- **Ver personas:** muestra los registros almacenados y permite actualizar la lista.
- **Editar persona:** permite cargar un registro y modificar sus datos.
- **Eliminar persona:** permite eliminar un registro utilizando su número de índice.
- **Exportar a CSV:** permite descargar los registros en un archivo `personas.csv`.

## Validaciones

El sistema realiza algunas validaciones antes de guardar los datos:

- Los campos de nombre, apellido y ciudad no pueden estar vacíos.
- La edad debe ser un número.
- La edad debe estar entre 1 y 120 años.
- El índice utilizado para editar o eliminar debe corresponder a un registro existente.

## Tecnologías utilizadas

- **Python**
- **Google Colab**
- **Gradio**
- **CSV**

# Autores
Valery Montes Echaves y Jose Gabriel Plata Ariza
