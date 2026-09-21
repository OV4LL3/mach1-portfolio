# MACH 1 — Plataforma de Procesamiento y Análisis de Datos Financieros

**Proyecto de portafolio | Python · Procesamiento de datos · Backend · Analytics**

MACH 1 es un proyecto personal de ingeniería de software diseñado para transformar información contenida en estados de cuenta bancarios en formato PDF en datos estructurados, validados y preparados para su análisis.

El proyecto trabaja sobre un flujo completo de datos:

**Carga de PDF → extracción → transformación → validación → persistencia → análisis → visualización**

> Este repositorio es un caso de estudio público del proyecto MACH 1.
> El código fuente completo y los datos financieros utilizados durante el desarrollo permanecen en un repositorio privado.

---

## 🎯 Objetivo del proyecto

Los estados de cuenta contienen información financiera importante, pero normalmente están diseñados para ser leídos por personas y no para ser procesados automáticamente.

MACH 1 fue creado para investigar y desarrollar una solución capaz de convertir estos documentos en información financiera estructurada que posteriormente pueda utilizarse para:

* Analizar movimientos financieros.
* Identificar ingresos y gastos.
* Construir dashboards financieros.
* Consultar históricos por cuenta.
* Validar información extraída.
* Analizar tendencias financieras.
* Servir como base para futuras herramientas de apoyo a la toma de decisiones.

---

## ⚙️ Flujo principal de datos

```text
Estado de cuenta bancario PDF
            │
            ▼
Validación del archivo
            │
            ▼
Extracción de información
            │
            ▼
Detección de institución bancaria
            │
            ▼
Parser específico
            │
            ▼
Limpieza y normalización
            │
            ▼
Procesamiento con pandas / DataFrames
            │
            ▼
Validación y enriquecimiento
            │
            ▼
Persistencia en PostgreSQL
            │
            ▼
API REST
            │
            ▼
Analytics y Dashboards
```

---

## 🧰 Tecnologías utilizadas

### Backend y procesamiento de datos

* Python
* Flask
* pandas
* PostgreSQL
* SQLAlchemy
* APIs REST

### Procesamiento documental

* pdfplumber
* OCR dirigido
* Parsers basados en reglas
* Normalización y validación de datos

### Calidad de software

* pytest
* Ruff
* Git
* GitHub Actions
* Pruebas automatizadas de regresión

### Frontend y visualización

* HTML
* CSS
* JavaScript
* Chart.js

### Tecnologías adicionales

* Alembic para migraciones de base de datos
* Configuración Docker
* Power BI *(actualmente en proceso de aprendizaje mediante un proyecto práctico de portafolio)*

---

## 🏗️ Arquitectura del software

MACH 1 utiliza una arquitectura por capas para separar responsabilidades y facilitar el mantenimiento, las pruebas y la evolución del sistema.

```text
Routes
   ↓
Services
   ↓
Repositories
   ↓
Models / Base de datos
```

Además, existen componentes especializados encargados de:

```text
Procesamiento de PDFs
Parsers bancarios
Extracción de información financiera
Identificación de cuentas
Validación de datos
Analytics
```

Esta separación permite modificar o mejorar componentes específicos sin acoplar excesivamente todo el sistema.

---

## 🔐 Privacidad y alcance de este repositorio

El código fuente completo de MACH 1 permanece en un repositorio privado debido a que el proyecto trabaja con procesamiento de documentación financiera y conjuntos de datos utilizados durante su desarrollo.

Este repositorio público tiene como objetivo documentar:

* La arquitectura del sistema.
* Las decisiones de ingeniería.
* Las tecnologías utilizadas.
* Los flujos de procesamiento de datos.
* Capturas y demostraciones del proyecto.
* Problemas técnicos encontrados y sus soluciones.
* La evolución del proyecto.

Aquí no se publican:

* Credenciales bancarias.
* Información financiera personal.
* Estados de cuenta reales.
* Contraseñas.
* Bases de datos privadas.
* Datos confidenciales.
