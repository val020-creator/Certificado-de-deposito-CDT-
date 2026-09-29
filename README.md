# 💰 Simulador de Certificado de Depósito a Término (CDT)

## 📌 Descripción

Este proyecto consiste en un programa desarrollado en **Python** que permite calcular y proyectar el saldo de un **Certificado de Depósito a Término (CDT)** a partir de un monto inicial y un plazo determinado en meses.

El programa calcula automáticamente la tasa de interés mensual de acuerdo con el plazo seleccionado y proyecta el crecimiento del dinero mes a mes, mostrando los intereses generados y el saldo acumulado.

---

## 🎯 Objetivo

Desarrollar un módulo que permita:

* Solicitar un monto inicial en pesos.
* Solicitar el plazo del CDT en meses.
* Validar que el monto sea mayor que `0`.
* Validar que el plazo sea un número entero mayor o igual a `1`.
* Calcular la tasa mensual según el plazo.
* Calcular los intereses generados cada mes.
* Proyectar el saldo acumulado durante todo el plazo.
* Mostrar una tabla con la evolución mensual del CDT.
* Mostrar el saldo final y el total de dinero ganado.

---

## 📐 Fórmula utilizada

La tasa mensual se calcula mediante la siguiente fórmula:

```text
tasaMensual (%) = 0,001695 × plazo + 0,0983
```

Para cada mes se calcula el interés mediante:

```text
interes = saldoAnterior × (tasaMensual / 100)
```

Posteriormente, se actualiza el saldo:

```text
saldoNuevo = saldoAnterior + interes
```

La tasa calculada según el plazo se mantiene constante durante toda la proyección.

---

## ⚙️ Funcionamiento

El programa sigue el siguiente proceso:

```text
Inicio
  ↓
Solicitar monto inicial
  ↓
¿Monto > 0?
  ├── No → Mostrar error y volver a solicitar
  └── Sí
        ↓
Solicitar plazo
        ↓
¿Plazo >= 1 y es entero?
  ├── No → Mostrar error y volver a solicitar
  └── Sí
        ↓
Calcular tasa mensual
        ↓
Inicializar saldo
        ↓
Calcular interés de cada mes
        ↓
Actualizar saldo
        ↓
Guardar resultados
        ↓
Mostrar tabla mensual
        ↓
Mostrar saldo final y total ganado
        ↓
Fin
```

---

## 📊 Información mostrada

La tabla de resultados contiene:

| Campo       | Descripción                          |
| ----------- | ------------------------------------ |
| **Mes**     | Número del mes de la proyección      |
| **Interés** | Dinero generado durante ese mes      |
| **Saldo**   | Dinero acumulado al finalizar el mes |

El **mes 0** corresponde al momento inicial del CDT, antes de generar intereses.

---

## 🛡️ Validaciones

El programa cuenta con validaciones para evitar datos incorrectos:

### Monto inicial

Debe ser un número mayor que `0`.

Ejemplo válido:

```text
Ingrese el monto inicial en pesos: $1000000
```

Ejemplos no válidos:

```text
-500000
0
```

### Plazo

Debe ser un número entero mayor o igual a `1`.

Ejemplo válido:

```text
Ingrese el plazo en meses: 12
```

Ejemplos no válidos:

```text
0
-5
2.5
```

Si se introduce un valor incorrecto, el programa muestra un mensaje de error y vuelve a solicitar el dato.

---

## 🧮 Ejemplo

Si el usuario ingresa:

```text
Monto inicial: $1.000.000
Plazo: 12 meses
```

El programa calcula primero la tasa mensual:

```text
tasaMensual = 0,001695 × 12 + 0,0983
```

Después realiza el cálculo correspondiente para cada uno de los 12 meses y muestra la evolución del saldo.

Al finalizar, se presenta:

```text
Monto inicial
Plazo
Tasa mensual
Saldo final
Total ganado
```

---

## 💻 Tecnologías utilizadas

* **Python 3**
* Estructuras de control `while` y `for`
* Manejo de excepciones con `try` / `except`
* Listas para almacenar resultados
* Operaciones matemáticas
* Formateo de datos para presentación en consola

---

## 📁 Estructura del proyecto

```text
CDT/
│
├── CDT.py
└── README.md
```

### `CDT.py`

Contiene el código principal del simulador del Certificado de Depósito a Término.

### `README.md`

Contiene la documentación, descripción, fórmulas, funcionamiento y validaciones del proyecto.

---

## 🚀 Ejecución

1. Descargar o clonar el repositorio.
2. Abrir el archivo `CDT.py`.
3. Ejecutar el programa utilizando Python 3.
4. Ingresar el monto inicial.
5. Ingresar el plazo en meses.
6. Consultar la proyección y el resultado final.

Para ejecutar desde una terminal:

```bash
python CDT.py
```

---

## 👨‍💻 Autores
Valery Montes Echavez y 
Jose Gabriel Plata Ariza
