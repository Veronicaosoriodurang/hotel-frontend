Grand Hotel - Frontend Independiente
=====================================

Frontend independiente para el sistema de gestion hotelera Grand Hotel.
Desarrollado con HTML, CSS y JavaScript puro sin frameworks ni dependencias.

---

1. Descripcion
--------------

Interfaz web independiente que consume la API REST del backend Spring Boot.
Permite gestionar clientes con CRUD completo:
listar, crear, editar y eliminar.

Este proyecto es completamente independiente del backend.
No requiere instalacion ni servidor propio.
Solo necesita que el backend este corriendo en localhost:8080.

---

2. Tecnologias
--------------

    HTML5       Estructura de la pagina
    CSS3        Estilos y diseno
    JavaScript  Logica y consumo de la API con fetch nativo

Sin frameworks, sin dependencias, sin instalacion.

---

3. Estructura del proyecto
---------------------------

    hotel-frontend/
        index.html    Aplicacion completa en un solo archivo
        README.md     Documentacion del proyecto

---

4. Funcionalidades
------------------

    Listar    Muestra todos los clientes al abrir la pagina
    Crear     Formulario para registrar un nuevo cliente
    Editar    Clic en Editar para cargar los datos y modificarlos
    Eliminar  Clic en Eliminar con confirmacion antes de borrar

---

5. Como usar
------------

Paso 1 - Iniciar el backend Spring Boot:
    cd C:\Users\Veroo\IdeaProjects\demo
    .\gradlew bootRun
    Esperar hasta ver: Tomcat started on port 8080

Paso 2 - Abrir el frontend:
    Ir a la carpeta C:\Users\Veroo\hotel-frontend
    Hacer doble clic en index.html
    O desde la terminal: start C:\Users\Veroo\hotel-frontend\index.html

Paso 3 - Usar la aplicacion:
    La pagina carga automaticamente la lista de clientes
    Llenar el formulario y dar clic en Guardar para crear un cliente
    Dar clic en Editar para modificar un cliente existente
    Dar clic en Eliminar para borrar un cliente

---

6. Endpoints que consume
------------------------

    GET    http://localhost:8080/api/clientes        Listar todos los clientes
    POST   http://localhost:8080/api/clientes        Crear nuevo cliente
    PUT    http://localhost:8080/api/clientes/{id}   Actualizar cliente
    DELETE http://localhost:8080/api/clientes/{id}   Eliminar cliente

Los datos que se envian al backend son:
    nombre   : texto
    apellido : texto
    email    : correo electronico

---

7. Repositorio del backend
---------------------------

El backend que consume este frontend esta en:
    https://github.com/Veronicaosoriodurang/demo

Tecnologias del backend:
    Spring Boot 3.5.11
    MySQL 8.0.45
    Patron DAO con PreparedStatement
    Swagger OpenAPI 2.8.5

---

8. Repositorios GitHub
-----------------------

    Frontend : https://github.com/Veronicaosoriodurang/hotel-frontend
    Backend  : https://github.com/Veronicaosoriodurang/demo

---

9. Autora
----------

    Veronica Osorio Durango
    Materia: Programacion de Software
    Programa: Tecnologia en Desarrollo de Software
    Institucion: ITM
    Periodo: 2026-1
    Entrega 4 - Frontend independiente