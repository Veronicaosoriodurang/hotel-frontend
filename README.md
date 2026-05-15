# Grand Hotel — Frontend

Frontend independiente del sistema de gestion hotelera Grand Hotel.
Desarrollado con HTML, CSS y JavaScript puro — sin frameworks ni dependencias.

> Este proyecto consume la API REST del backend. Ver: [demo (backend)](https://github.com/Veronicaosoriodurang/demo)

---

## Navegacion rapida

- [Como poner a funcionar](#como-poner-a-funcionar)
- [Que hace](#que-hace)
- [Como funciona](#como-funciona)
- [Endpoints que consume](#endpoints-que-consume)
- [Autora](#autora)

---

## Como poner a funcionar

**Paso 1 — Iniciar el backend**

```bash
cd demo
.\gradlew bootRun
```

Esperar hasta ver: `Tomcat started on port 8080`

**Paso 2 — Abrir el frontend**

Ir a la carpeta `hotel-frontend` y hacer doble clic en `index.html`.

O desde la terminal:

```bash
start index.html
```

**Listo.** La pagina carga automaticamente los clientes desde la API.

---

## Que hace

| Operacion | Descripcion |
|-----------|-------------|
| Listar | Muestra todos los clientes al abrir la pagina |
| Crear | Formulario para registrar un nuevo cliente |
| Editar | Clic en Editar para modificar un cliente |
| Eliminar | Clic en Eliminar con confirmacion |

---

## Como funciona

El frontend se comunica con el backend mediante `fetch` en JavaScript:

```
index.html abierto en el navegador
        |
        | fetch (HTTP)
        v
http://localhost:8080/api/clientes  (backend Spring Boot)
        |
        v
MySQL — base de datos hoteldb
```

No se conecta directamente a MySQL. Todo pasa por el backend.

---

## Endpoints que consume

| Metodo | URL | Accion |
|--------|-----|--------|
| GET | http://localhost:8080/api/clientes | Listar clientes |
| POST | http://localhost:8080/api/clientes | Crear cliente |
| PUT | http://localhost:8080/api/clientes/{id} | Actualizar cliente |
| DELETE | http://localhost:8080/api/clientes/{id} | Eliminar cliente |

**Datos que envia:**
```json
{
  "nombre": "texto",
  "apellido": "texto",
  "email": "correo@email.com"
}
```

---

## Estructura

```
hotel-frontend/
    index.html    Aplicacion completa en un solo archivo
    README.md     Esta documentacion
```

---

## Tecnologias

| Tecnologia | Uso |
|------------|-----|
| HTML5 | Estructura de la pagina |
| CSS3 | Estilos y diseno |
| JavaScript | Logica y consumo de la API |

Sin instalacion. Sin dependencias. Solo abrir el archivo.

---

## Backend

Este frontend requiere el backend corriendo. Ver instrucciones en:

[https://github.com/Veronicaosoriodurang/demo](https://github.com/Veronicaosoriodurang/demo)

---

## Autora

| | |
|-|-|
| Nombre | Veronica Osorio Durango |
| Materia | Programacion de Software |
| Programa | Tecnologia en Desarrollo de Software |
| Institucion | ITM |
| Periodo | 2026-1 |
