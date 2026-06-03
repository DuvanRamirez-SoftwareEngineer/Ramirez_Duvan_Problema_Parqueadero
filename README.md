# 🚗 Simulación del Sistema de Pago de Parqueaderos
## Centro Comercial Supercentro

---

## 📋 Descripción del Proyecto

Este proyecto corresponde a la Actividad Didáctica 2 del Módulo 4.

Se desarrolló una simulación del sistema de pago de parqueaderos del Centro Comercial Supercentro utilizando teoría de colas y el modelo M/M/1.

El objetivo principal es determinar si los tres cajeros disponibles son suficientes para atender la demanda actual o si es necesario implementar mejoras en el sistema.

---

# 🎯 Objetivos

## Objetivo General

Analizar el comportamiento del sistema de pago de parqueaderos mediante simulación para determinar la eficiencia de los cajeros actuales.

## Objetivos Específicos

- Simular un sistema de colas M/M/1.
- Identificar el cajero más eficiente.
- Identificar el cajero menos eficiente.
- Calcular el promedio de usuarios por tipo.
- Determinar el estado estable del sistema.
- Eliminar el estado transitorio.
- Aplicar verificación, calibración y validación.
- Formular estrategias de mejora.

---

# 🏢 Contexto del Problema

El Centro Comercial Supercentro cuenta con tres cajeros automáticos por salida.

Cada usuario debe:

1. Digitar la placa del vehículo.
2. Seleccionar el vehículo.
3. Realizar el pago.
4. Salir del parqueadero.

Los usuarios presentan diferentes velocidades de interacción con el sistema.

---

# 👥 Tipos de Usuarios

| Tipo | Servicio (min) | Llegada (min) | Probabilidad |
|--------|--------|--------|--------|
| Rápido | 1 | 3 | 25% |
| Normal | 3 | 3 | 20% |
| Lento | 4 | 5 | 27.5% |
| Muy Lento | 6 | 7 | 27.5% |

---

# 📚 Fundamento Teórico

Se utilizó el modelo M/M/1.

Características:

- Llegadas Poisson.
- Servicio exponencial.
- Un servidor.
- Cola FIFO.
- Capacidad infinita.

---

## Fórmulas Utilizadas

### Factor de Utilización

ρ = λ / μ

### Clientes Promedio en el Sistema

L = ρ / (1 − ρ)

### Clientes Promedio en Cola

Lq = ρ² / (1 − ρ)

### Tiempo Promedio en Sistema

W = 1 / (μ − λ)

### Tiempo Promedio en Cola

Wq = ρ / (μ − λ)

---

# 💻 Tecnologías Utilizadas

- Python
- Google Colab
- NumPy
- Pandas
- Matplotlib
- SciPy
- Excel

---

# 🔬 Metodología

## Paso 1

Definición de parámetros del problema.

## Paso 2

Generación de usuarios aleatorios.

## Paso 3

Simulación de tres cajeros M/M/1 independientes.

## Paso 4

Ejecución de múltiples réplicas.

## Paso 5

Determinación del estado estable.

## Paso 6

Eliminación del estado transitorio.

## Paso 7

Cálculo de estadísticas.

## Paso 8

Exportación de resultados a Excel.

---

# 📈 Resultados Obtenidos

Se calcularon:

✅ Tiempo promedio de atención por cajero.

✅ Desviación estándar.

✅ Intervalos de confianza del 95%.

✅ Promedio de usuarios por tipo.

✅ Porcentaje de usuarios observados.

✅ Tiempo promedio en el sistema.

✅ Tiempo promedio de espera.

✅ Utilización de los cajeros.

---

# 📊 Gráficas Generadas

El proyecto genera automáticamente:

### 1. Estado Estable

Determinación del período de calentamiento mediante promedio móvil.

### 2. Antes y Después del Estado Transitorio

Comparación de los datos originales y depurados.

### 3. Tiempo Promedio por Cajero

Identificación del cajero más eficiente.

### 4. Usuarios por Tipo

Distribución de usuarios rápidos, normales, lentos y muy lentos.

### 5. Tiempo Promedio por Tipo

Comparación de tiempos entre categorías de usuarios.

### 6. Proceso de Verificación, Calibración y Validación

Diagrama del proceso V&V.

---

# 🔍 Verificación

Se verificó:

- Correcta generación de usuarios.
- Correcta generación exponencial.
- Correcta asignación de cajeros.
- Correcta captura de estadísticas.
- Correcta exportación de datos.

---

# ⚙️ Calibración

Los parámetros utilizados corresponden exactamente a los valores definidos en el enunciado.

---

# ✅ Validación

El modelo fue comparado con la teoría de colas M/M/1.

Se verificó:

- Estabilidad del sistema.
- Coherencia estadística.
- Comportamiento esperado.

---

# 📁 Archivos del Repositorio

```text
📂 Proyecto_Parqueadero

 Ramirez_Duvan_problemaParqueadero.docx
```

---

# ▶️ Ejecución

Abrir:

```text
Ramirez_Duvan_problemaParqueadero.ipynb
```

Ejecutar todas las celdas de Google Colab.

El sistema generará automáticamente:

- Tablas.
- Estadísticas.
- Gráficas.
- Archivo Excel.

---

# 📦 Salidas Generadas

## Excel

```text
Ramirez_Duvan_Resultados_Parqueadero.xlsx
```

Contiene:

- Datos simulados.
- Estadísticas por cajero.
- Usuarios por tipo.
- Intervalos de confianza.

---

# 👨‍💻 Autor

Nombre: Duván Oswaldo Ramírez Duarte

---

# ⭐ Conclusión General

La simulación permitió analizar el desempeño del sistema de pago de parqueaderos, identificar oportunidades de mejora y apoyar la toma de decisiones mediante evidencia estadística obtenida a partir de modelos de colas M/M/1.
