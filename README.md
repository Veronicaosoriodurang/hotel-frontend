Grand Hotel - Frontend
======================

Frontend independiente para el sistema de gestion hotelera Grand Hotel.
Desarrollado con HTML, CSS y JavaScript puro sin frameworks.

---

1. Descripcion
--------------

Interfaz web que consume la API REST del backend Spring Boot.
Permite gestionar clientes con operaciones de consulta, creacion,
actualizacion y eliminacion (CRUD completo).

---

2. Tecnologias
--------------

    HTML5       Estructura de la pagina
    CSS3        Estilos y diseno responsive
    JavaScript  Logica y consumo de la API con fetch

---

3. Funcionalidades
------------------

    Listar    Muestra todos los clientes registrados
    Crear     Formulario para registrar un nuevo cliente
    Editar    Permite modificar los datos de un cliente
    Eliminar  Elimina un cliente con confirmacion

---

4. Como usar
------------

Requisitos:
    - Tener el backend corriendo en http://localhost:8080
    - Abrir el archivo index.html en el navegador

Pasos:
    1. Iniciar el backend Spring Boot
    2. Abrir index.html en el navegador
    3. La aplicacion se conecta automaticamente a la API

---

5. Endpoints que consume
------------------------

    GET    http://localhost:8080/api/clientes        Listar clientes
    POST   http://localhost:8080/api/clientes        Crear cliente
    PUT    http://localhost:8080/api/clientes/{id}   Actualizar cliente
    DELETE http://localhost:8080/api/clientes/{id}   Eliminar cliente

---

6. Repositorio del backend
---------------------------

    https://github.com/Veronicaosoriodurang/demo

---

7. Autora
---------

    Veronica Osorio Durango
    Materia: Programacion de Software
    Programa: Tecnologia en Desarrollo de Software
    Institucion: ITM
    Periodo: 2026-1
    Entrega 4 - Semana 20