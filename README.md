# 📚 Guía para Documentar APIs con Swagger Editor (Sin Instalación) 🌐

## Introducción

Bienvenido a esta guía práctica sobre cómo documentar tus APIs utilizando **Swagger Editor** sin necesidad de instalar nada en tu ordenador. Swagger Editor es una herramienta poderosa que te permite diseñar, construir y documentar APIs de manera interactiva. 

## 🛠️ Requisitos Previos

Antes de comenzar, asegúrate de tener lo siguiente:
- Un navegador web actualizado (Chrome, Firefox, Safari, etc.).
- Conexión a internet.

## 🚀 Pasos para Usar Swagger Editor

### 1. Acceder a Swagger Editor

Para acceder a Swagger Editor, simplemente visita la siguiente URL: 

👉 [**Swagger Editor**](https://editor.swagger.io/) 👈

### 2. Entorno del Editor

Al abrir Swagger Editor, verás una interfaz dividida en dos paneles:
- **Panel Izquierdo:** Donde escribirás el código YAML para definir tu API.
- **Panel Derecho:** Vista previa interactiva de la documentación generada.

![Swagger Editor Interface](https://user-images.githubusercontent.com/25639885/120939613-7740c080-c6e1-11eb-9f37-1f08e8d8f9f8.png)

### 3. Crear una API Básica

Puedes comenzar con una plantilla básica que Swagger Editor proporciona por defecto. Para empezar desde cero, elimina el contenido existente y utiliza el siguiente ejemplo mínimo:

```yaml
openapi: 3.0.0
info:
  title: Mi API de Ejemplo
  description: Una API sencilla para demostrar Swagger Editor.
  version: 1.0.0
paths:
  /saludo:
    get:
      summary: Devuelve un saludo
      responses:
        '200':
          description: Éxito
          content:
            application/json:
              schema:
                type: object
                properties:
                  mensaje:
                    type: string
                    example: "Hola, mundo!"
