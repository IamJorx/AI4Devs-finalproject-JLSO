> Detalla en esta sección los prompts principales utilizados durante la creación del proyecto, que justifiquen el uso de asistentes de código en todas las fases del ciclo de vida del desarrollo. Esperamos un máximo de 3 por sección, principalmente los de creación inicial o los de corrección o adición de funcionalidades que consideres más relevantes.
> Puedes añadir adicionalmente la conversación completa como link o archivo adjunto si así lo consideras

## Índice

1. [Descripción general del producto](#1-descripción-general-del-producto)
2. [Arquitectura del sistema](#2-arquitectura-del-sistema)
3. [Modelo de datos](#3-modelo-de-datos)
4. [Especificación de la API](#4-especificación-de-la-api)
5. [Historias de usuario](#5-historias-de-usuario)
6. [Tickets de trabajo](#6-tickets-de-trabajo)
7. [Pull requests](#7-pull-requests)

---

## 1. Descripción general del producto

**Prompt 1:**

```
# Contexto del Proyecto
Estoy desarrollando un sistema basado en IA para analizar y comparar transacciones bancarias de archivos Excel. El sistema debe:
1. Permitir la carga de dos archivos Excel con registros de transacciones bancarias.
2. Analizar y encontrar coincidencias entre las transacciones basadas en ciertos criterios clave (id_transaccion, fecha, cuenta_origen, cuenta_destino, monto).
3. Detectar discrepancias en los estados de las transacciones (Ej: Exitosa vs Fallida).
4. Resolver problemas comunes como:
   - Diferencias en nombres de columnas (id_transaccion vs id de transacción).
   - Formatos de fecha distintos (2025-02-10 vs 10/02/2025).
   - Variaciones menores en los montos ($500.00 vs 500,00).

# Implementación
Estoy utilizando IA para mejorar la comparación de transacciones cuando los datos no coinciden exactamente. La arquitectura actual del proyecto incluye:
- **Python + Pandas** para procesamiento de datos.
- **FAISS (Facebook AI Similarity Search)** para buscar transacciones similares usando embeddings.
- **SentenceTransformers (BERT, MiniLM, etc.)** para generar embeddings de transacciones.
- **Excel como formato de entrada y salida**, con un archivo final que contiene:
   - **Coincidencias exactas** de transacciones.
   - **Coincidencias con discrepancias** en estado/monto.
   - **Registros que deben revisarse manualmente**.

# Objetivo
El objetivo es seguir desarrollando este sistema, optimizando su precisión y eficiencia. Quiero que ChatGPT continúe ayudándome con:
- Mejoras en el código y optimización del pipeline.
- Evaluación de rendimiento de FAISS y embeddings.
- Implementación de una API para integrar el procesamiento en una app web.
- Pruebas con datos reales y detección de errores.
- Recomendaciones de herramientas y mejoras en la lógica de comparación.

# Preferencias
- Quiero que ChatGPT recuerde el contexto del proyecto y proponga soluciones basadas en las tecnologías mencionadas.
- Si hay una forma más eficiente de implementar algo, quiero sugerencias específicas con código.
- Si alguna parte del pipeline puede mejorarse con otro enfoque, quiero entender **por qué y cómo** hacerlo.
- Prefiero soluciones que puedan escalar bien si trabajo con archivos grandes.
```

**Prompt 2:**

```
Ahora tenemos que empezar a construir la documentación del proyecto, para cada sección hay que registrar los prompt utilizados para construir esa parte de la documentación. Aquí están los formatos de la documentación del proyecto y de el archivo donde se van a documentar los prompts utilizados, aún no empieces a sugerir nada, pues iremos paso a paso según lo indique.
```

**Prompt 3:**

```
Empecemos con la documentación, por la primera parte del proyecto "descripción breve del proyecto", en base a la documentación y contexto proporcionado, sugiere:
1. una descripción breve del proyecto, el proyecto tiene como nombre "Close AI"
2. Objetivo:
   - Propósito del producto. Qué valor aporta, qué soluciona, y para quién.
3. Características y funcionalidades principales:
   - Enumera y describe las características y funcionalidades específicas que tiene el producto para satisfacer las necesidades identificadas.
4. Diseño y experiencia de usuario:
   - Proporciona imágenes y/o videotutorial mostrando la experiencia del usuario desde que aterriza en la aplicación, pasando por todas las funcionalidades principales.
5. Instrucciones de instalación:
   - Documenta de manera precisa las instrucciones para instalar y poner en marcha el proyecto en local (librerías, backend, frontend, servidor, base de datos, migraciones y semillas de datos, etc.)
   - El frontend será una aplicación en next y el backend una api en fastapi
   - Base de datos: postgresql
```

---

## 2. Arquitectura del Sistema

### **2.1. Diagrama de arquitectura:**

**Prompt 1:**

```
Ahora continuaremos con la documentación, por la sección "Diagrama de arquitectura", en base a la documentación y contexto proporcionado, sugiere:
1. Un diagrama de arquitectura del proyecto, que muestre los componentes principales y su interacción.
2. Una descripción de cada componente y su responsabilidad.
3. Las tecnologías y herramientas que se utilizarán para cada componente.

usa el formato que consideres más adecuado para representar los componentes principales de la aplicación y las tecnologías utilizadas. Explica si sigue algún patrón predefinido, justifica por qué se ha elegido esta arquitectura, y destaca los beneficios principales que aportan al proyecto y justifican su uso, así como sacrificios o déficits que implica.

Usa la estrategia DaC (document as code) para generar el diagrama de arquitectura.

Antes de empezar sugiere que formatos de DaC podríamos utilizar para generar el diagrama de arquitectura.
```

**Prompt 2:**

```

```

**Prompt 3:**

```

```

### **2.2. Descripción de componentes principales:**

**Prompt 1:**

```

```

**Prompt 2:**

```

```

**Prompt 3:**

```

```

### **2.3. Descripción de alto nivel del proyecto y estructura de ficheros**

**Prompt 1:**

```

```

**Prompt 2:**

```

```

**Prompt 3:**

```

```

### **2.4. Infraestructura y despliegue**

**Prompt 1:**

```

```

**Prompt 2:**

```

```

**Prompt 3:**

```

```

### **2.5. Seguridad**

**Prompt 1:**

```

```

**Prompt 2:**

```

```

**Prompt 3:**

```

```

### **2.6. Tests**

**Prompt 1:**

```

```

**Prompt 2:**

```

```

**Prompt 3:**

```

```

---

### 3. Modelo de Datos

**Prompt 1:**

```

```

**Prompt 2:**

```

```

**Prompt 3:**

```

```

---

### 4. Especificación de la API

**Prompt 1:**

```

```

**Prompt 2:**

```

```

**Prompt 3:**

```

```

---

### 5. Historias de Usuario

**Prompt 1:**

```

```

**Prompt 2:**

```

```

**Prompt 3:**

```

```

---

### 6. Tickets de Trabajo

**Prompt 1:**

```

```

**Prompt 2:**

```

```

**Prompt 3:**

```

```

---

### 7. Pull Requests

**Prompt 1:**

```

```

**Prompt 2:**

```

```

**Prompt 3:**

```

```
