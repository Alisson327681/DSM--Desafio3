# 📚 AprendeApp – Sistema de Gestión de Recursos de Aprendizaje

Aplicación móvil Android desarrollada como parte del **Tercer Desafío Práctico** de la asignatura Desarrollo de Software para Móviles (DSM), de la Universidad Don Bosco.

AprendeApp es una aplicación diseñada para gestionar recursos educativos relacionados con Ingeniería de Sistemas, permitiendo a estudiantes y docentes consultar, organizar y administrar materiales de aprendizaje como libros, videos, artículos y tutoriales.

---

## 🎯 Objetivo del proyecto

Desarrollar una aplicación móvil que facilite el acceso y la administración de recursos educativos mediante una interfaz intuitiva, utilizando una API dinámica para la gestión de información y una arquitectura MVC que permita organizar el código de manera estructurada.

## 🛠️ Tecnologías utilizadas

- **Lenguaje:** Kotlin.
- **Entorno de desarrollo:** Android Studio.
- **Arquitectura:** MVC (Model - View - Controller).
- **API REST:** MockAPI.io o Railway.
- **Formato de intercambio de datos:** JSON.
- **Almacenamiento:** Persistencia de datos de usuario.
- **Interfaz:** Componentes visuales de Android.

## 👥 Roles de usuario

La aplicación contempla dos tipos de usuarios:

### 🎓 Estudiante
- Iniciar sesión en la aplicación.
- Visualizar los recursos educativos disponibles.
- Buscar recursos por ID, título o tipo.
- Filtrar y ordenar los recursos.
- Agregar recursos a favoritos.
- Calificar recursos mediante un sistema de estrellas de 1 a 5.

### 👨‍🏫 Docente
- Iniciar sesión con permisos de docente.
- Visualizar los recursos educativos.
- Agregar nuevos recursos.
- Editar información de los recursos existentes.
- Eliminar recursos con confirmación.
- Administrar la lista principal de recursos mediante operaciones CRUD.

## ⚙️ Funcionalidades principales

### 1. Registro e inicio de sesión
- Registro de nuevos usuarios.
- Inicio y cierre de sesión.
- Validación de contraseñas seguras.
- Autenticación mediante roles.

**Requisitos de contraseña:**
- Mínimo 12 caracteres.
- Al menos una letra mayúscula.
- Al menos una letra minúscula.
- Al menos un número.
- Al menos un carácter especial.

### 2. Gestión de recursos educativos
La aplicación permite administrar recursos mediante una API REST.

Cada recurso puede contener:
- ID.
- Título.
- Descripción.
- Tipo de recurso.
- Enlace.
- Imagen ilustrativa.

### 3. Operaciones CRUD

| Operación | Descripción |
|---|---|
| GET | Consultar recursos. |
| POST | Agregar recursos. |
| PUT | Modificar recursos. |
| DELETE | Eliminar recursos. |

### 4. Búsqueda y filtros
- Búsqueda por identificador.
- Búsqueda por título.
- Búsqueda por tipo de recurso.
- Ordenamiento y filtrado de información.

### 5. Favoritos
Permite guardar recursos educativos seleccionados por cada usuario y consultar posteriormente su lista personalizada de favoritos.

### 6. Sistema de calificaciones
Permite a los estudiantes calificar los recursos mediante una escala de 1 a 5 estrellas, mostrando el promedio de las valoraciones.

## 🏗️ Arquitectura MVC

El proyecto utiliza el patrón de arquitectura MVC para organizar sus componentes:

- **Model:** administra los datos y la lógica relacionada con los recursos y usuarios.
- **View:** contiene las interfaces y elementos visuales que utiliza el usuario.
- **Controller:** gestiona las acciones del usuario y conecta las vistas con los modelos y los servicios de datos.

## 🌐 API y datos dinámicos

La aplicación utiliza una API externa para consultar y administrar los recursos educativos en formato JSON.

Cada operación permite mantener la información actualizada y sincronizada con el servicio de datos.

**Ejemplo de estructura JSON:**

```json
{
  "id": 1,
  "titulo": "Introducción a Kotlin",
  "descripcion": "Material de aprendizaje sobre Kotlin.",
  "tipo": "Tutorial",
  "enlace": "https://example.com",
  "imagen": "https://example.com/imagen.jpg"
}
```

## 📱 Interfaz de usuario

La aplicación busca ofrecer una experiencia de usuario:

- Clara e intuitiva.
- Adaptable a dispositivos Android.
- Con navegación sencilla.
- Con mensajes de confirmación y alertas.
- Con indicadores de carga y retroalimentación visual.

## 🚀 Instalación y ejecución

Para ejecutar el proyecto 