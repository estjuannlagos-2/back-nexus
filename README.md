# 🔧 Backend – Nexus API

Este repositorio contiene la implementación del backend del sistema, diseñado bajo una arquitectura modular que soporta dos tecnologías distintas para el manejo de la lógica del servidor y la persistencia de datos.

👥 Integrantes

David Esteban Avila Rojas – 1202775

Juan Nicolás Lagos Fuquen – 1202737

David Felipe Alvarado Romero – 1202727

## 🎯 Objetivo

Desarrollar una infraestructura de servidor capaz de:

* Gestionar y procesar solicitudes HTTP.
* Implementar operaciones **CRUD** (Create, Read, Update, Delete) completas.
* Establecer conexión robusta con la base de datos.
* Garantizar respuestas estandarizadas en formato **JSON**.

---

## 🌿 Estructura de Ramas

El proyecto está organizado en ramas independientes según la tecnología implementada:

### 🟢 Rama: `node-version`

Backend desarrollado con **Node.js** (arquitectura nativa/sin frameworks).

* **Ejecución Local:** ```bash
npm install
npm start
```

```


* **Servidor local:** `http://localhost:3000`
* **Despliegue:** Compatible con Render, Railway, VPS.
* **Configuración:** Utiliza `const PORT = process.env.PORT || 3000;` para entornos en la nube.

### 🔵 Rama: `php-version`

Backend desarrollado con **PHP** bajo una estructura modular.

* **Ejecución Local:** ```bash
php -S localhost:8000
```

```


* **Servidor local:** `http://localhost:8000`
* **Despliegue:** Compatible con InfinityFree, Hostinger, Render, XAMPP.

---

## 📡 Endpoints Implementados

| Método | Ruta | Descripción |
| --- | --- | --- |
| **GET** | `/api/users` | Obtener listado de usuarios |
| **POST** | `/api/users` | Crear un nuevo usuario |
| **PUT** | `/api/users/{id}` | Actualizar datos de un usuario |
| **DELETE** | `/api/users/{id}` | Eliminar un usuario |

---

## 🗄️ Base de Datos

El modelo de datos es unificado. El script de creación de tablas se encuentra disponible en:

> `/database/script.sql`

## 🔐 Validaciones y Seguridad

Para garantizar la integridad de los datos, se han implementado las siguientes reglas:

* **Campos obligatorios:** Verificación de presencia de datos clave.
* **Integridad:** Validación de formato para correos electrónicos.
* **Estándares:** Manejo estricto de códigos de estado **HTTP** y respuestas **JSON**.
* **CORS:** Configuración de cabeceras para permitir comunicación con el frontend.

---

## 🌍 URLs en Producción

| Versión | URL de Producción |
| --- | --- |
| **Node.js** | [https://nombre-app-node.onrender.com](https://nombre-app-node.onrender.com) |
| **PHP** | [https://back-nexus-production.up.railway.app](https://www.google.com/search?q=https://back-nexus-production.up.railway.app) |

---

*Proyecto desarrollado para la asignatura de Tecnologías del Internet.*
