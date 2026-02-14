# CRUD Productos – Spring Boot

Este proyecto consiste en una API REST desarrollada con Spring Boot que implementa un CRUD completo para la entidad Productos.  
La aplicación está conectada a una base de datos MySQL ejecutándose en un contenedor Docker.

---

## Objetivo del proyecto

El objetivo fue comprender cómo construir una API backend real utilizando arquitectura en capas, conexión a base de datos y pruebas con Postman.

Se trabajó desde cero:

- Configuración de Docker
- Configuración de MySQL
- Creación del proyecto con Spring Boot
- Implementación de arquitectura en capas
- Pruebas de endpoints

---

## Tecnologías utilizadas

- Java 17
- Spring Boot
- Spring Data JPA
- Hibernate (ORM)
- MySQL
- Docker
- Maven
- Postman

---

## Arquitectura del proyecto

El proyecto sigue una estructura en capas:

- Entity → Representa la tabla en la base de datos
- Repository → Acceso a datos con JpaRepository
- Service → Lógica de negocio
- Controller → Endpoints REST

---

## Endpoints implementados

Base URL: http://localhost:8080/api/productos


Operaciones disponibles:

- GET /api/productos → Listar todos los productos
- GET /api/productos/{id} → Buscar producto por ID
- POST /api/productos → Crear producto
- PUT /api/productos/{id} → Actualizar producto
- DELETE /api/productos/{id} → Eliminar producto

---

## Pruebas realizadas

Se utilizó Postman para validar cada endpoint:

1. GET inicial vacío
2. POST para insertar datos
3. GET para verificar inserción
4. PUT para actualizar datos
5. DELETE para eliminar registro

La colección exportada se encuentra en: CRUD_collection.json

---

## Cómo ejecutar el proyecto

1. Levantar el contenedor MySQL con Docker.
2. Verificar que el puerto 3307 esté disponible.
3. Ejecutar la aplicación Spring Boot.
4. Probar los endpoints con Postman.

---

Este proyecto representa la implementación básica de una API REST funcional conectada a base de datos utilizando separación en capas.