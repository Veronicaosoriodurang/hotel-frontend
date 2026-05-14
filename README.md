# Grand Hotel — Frontend

Frontend **independiente** del backend para el sistema hotelero **Grand Hotel**. Está construido solo con **HTML, CSS y JavaScript** (sin frameworks ni bundlers) y consume la API REST del backend **Spring Boot** en ejecución local.

## Requisitos

- Backend Spring Boot accesible en **`http://localhost:8080`**, con endpoints REST bajo **`/api`**:
  - **Clientes:** `GET/POST` `http://localhost:8080/api/clientes`, `GET/PUT/DELETE` `http://localhost:8080/api/clientes/{id}`
  - **Habitaciones:** `GET/POST` `http://localhost:8080/api/habitaciones`, `GET/PUT/DELETE` `http://localhost:8080/api/habitaciones/{id}`
  - **Reservas:** `GET` `http://localhost:8080/api/reservas` (el panel solo lista reservas)

## Cómo usarlo

1. Arranque el backend en el puerto **8080**.
2. Abra **`index.html`** en el navegador:
   - Puede abrir el archivo directamente desde el disco, o
   - Servir la carpeta con cualquier servidor estático (por ejemplo `npx serve .` o la extensión “Live Server” de VS Code) para evitar limitaciones de algunos navegadores con `file://` y **CORS**.

## CORS

Si abre `index.html` como archivo local o desde otro origen distinto de `http://localhost:8080`, el backend debe permitir el origen del frontend (cabeceras **CORS** en Spring Boot). Si sirve el HTML desde el mismo host y puerto que la API, CORS suele ser menos problemático.

## Contenido del panel

- **Clientes:** listado en tabla, formulario para crear y editar, eliminación con confirmación, mensajes de éxito y error.
- **Habitaciones:** igual, CRUD completo.
- **Reservas:** solo lectura — listado desde la API.

Los nombres de campos JSON del formulario (`nombre`, `apellidos`, `email`, `telefono`, `documento` para clientes; `numero`, `tipo`, `precio`, `disponible` para habitaciones) están pensados para un API típico. Si sus entidades DTO usan otros nombres, adapte el cuerpo enviado en el `<script>` de `index.html` para que coincida con su backend.

## Estructura del repositorio

```
hotel-frontend/
├── index.html    # Aplicación completa (estilos + lógica)
└── README.md
```

Listo para publicar como **repositorio independiente** en GitHub: cree un repositorio nuevo, suba estos archivos y opcionalmente añada una licencia o `.gitignore` según su equipo.

## Licencia

Sin licencia explícita por defecto; añada la que corresponda a su proyecto.
