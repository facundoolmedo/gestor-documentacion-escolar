# Gestor de Documentación Escolar

Centraliza y digitaliza la gestión de documentos escolares (boletines, permisos, recordatorios, pagos, comunicaciones y más) para familias, docentes y directivos. Proyecto pensado para escuelas argentinas, adaptable a diferentes niveles educativos.

---

## Stack Tecnológico

- **Backend:** Python + Django (REST API)
- **Frontend:** React (web/mobile-ready)
- **Base de Datos:** MySQL
- **Autenticación:** JWT (JSON Web Token)
- **Notificaciones:** SendGrid (email), Twilio (WhatsApp)
- **Infraestructura:** Docker Compose (orquestación de servicios)

---

## Estructura del proyecto

```plaintext
.
├── backend/         # Django API REST
├── frontend/        # React app
├── docker-compose.yml
├── README.md
└── docs/            # Wireframes y documentación de arquitectura
```

---

## Cómo levantar el entorno localmente

### 1. Clona el repositorio

```bash
git clone https://github.com/facundoolmedo/gestor-documentacion-escolar.git
cd gestor-documentacion-escolar
```

### 2. Configura las variables de entorno

Completa los archivos `.env` en `/backend` y `/frontend` con tus claves (MySQL, JWT_SECRET, SendGrid, Twilio, etc).

### 3. Levanta los servicios con Docker Compose

```bash
docker-compose up --build
```

Esto levanta:

- Django backend en `localhost:8000`
- React frontend en `localhost:3000`
- MySQL en `localhost:3306`

---

## Scripts útiles

- `docker-compose up --build`: Construye y levanta todo el stack.
- `docker-compose down`: Detiene y elimina los contenedores.
- `docker-compose logs -f backend`: Muestra logs del backend.

---

## Estructura base

- `/backend/`: Código fuente Django, settings, apps, tests, Dockerfile.
- `/frontend/`: Código fuente React, componentes, Dockerfile.
- `/docs/`: Wireframes, arquitectura, modelos de datos.

---

## Próximos pasos

- Definir modelos y endpoints básicos en Django.
- Crear pantallas dummy en React.
- Wireframes y arquitectura en `/docs`.

---

## Colaboradores

- [facundoolmedo](https://github.com/facundoolmedo)

---

## Licencia

MIT