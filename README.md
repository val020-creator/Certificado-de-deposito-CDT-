# 💰 Calculador de Certificado de Depósito a Término (CDT)

Aplicación desarrollada en **Python** que permite calcular y proyectar el crecimiento de un **Certificado de Depósito a Término (CDT)** durante un plazo determinado.

El sistema utiliza una interfaz gráfica desarrollada con **Gradio** y permite realizar operaciones de registro, consulta, edición, eliminación y exportación de los CDTs.

---

## 📌 Descripción del proyecto

Un Certificado de Depósito a Término (CDT) es un producto financiero en el que una persona deposita una cantidad de dinero durante un plazo determinado, generando intereses durante ese período.

Este proyecto permite ingresar:

- Monto inicial del CDT.
- Plazo en meses.

A partir de estos datos, el sistema calcula la tasa mensual y genera una proyección del saldo para cada mes del plazo seleccionado.

Los cálculos internos mantienen todos los decimales disponibles. Los valores mostrados en la interfaz se presentan redondeados a **dos decimales**.

---

## 🎯 Objetivo

Desarrollar una aplicación sencilla que permita registrar y administrar CDTs, calcular su crecimiento mensual y visualizar la proyección del saldo mediante una interfaz gráfica.

---

## ⚙️ Funcionalidades

El sistema cuenta con las siguientes opciones:

### ➕ Agregar

Permite registrar un nuevo CDT ingresando:

- Monto inicial.
- Plazo en meses.

El sistema calcula automáticamente la tasa mensual y genera la proyección del CDT.

---

### 👁️ Ver / Imprimir proyección

Permite seleccionar un CDT mediante su ID y visualizar su proyección mensual.

La tabla muestra:

| Campo | Descripción |
|---|---|
| Mes | Número del mes de la proyección |
| Interés | Interés generado durante el mes |
| Saldo | Saldo acumulado |

Los valores monetarios se muestran con dos decimales.

---

### ✏️ Editar

Permite modificar los datos de un CDT existente utilizando su ID.

Al realizar la modificación, el sistema genera nuevamente la proyección con los nuevos datos.

---

### 🗑️ Eliminar

Permite eliminar un CDT registrado utilizando su ID.

Después de eliminarlo, la tabla principal se actualiza automáticamente.

---

### 📥 Descargar CSV

Permite exportar los CDTs registrados a un archivo llamado:

```text
cdt.csv
```
---
## Autores

- Valery Montes Echavez  - 01240372023
- Jose Gabriel Plata Ariza - 01240372047
