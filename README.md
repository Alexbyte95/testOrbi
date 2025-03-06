# Testorbi

Este proyecto contiene dos microservicios (`service-a` y `service-b`) que se comunican mediante gRPC, HTTP y RabbitMQ.  

Incluye configuración para ejecutar los servicios tanto en local como en contenedores Docker.

## 📂 Repositorios

- **Proyecto raíz:** [TestOrbi](https://github.com/Alexbyte95/testOrbi/tree/configuration-initial)
- **Submódulos:**
  - [TestUserService](https://github.com/Alexbyte95/testUserService/)
  - [TestNotificationService](https://github.com/Alexbyte95/testNotificationService/)

---

## 📦 Requisitos previos

Asegúrate de tener instalado:

- [Node.js 20+](https://nodejs.org/)
- [npm](https://www.npmjs.com/) o [yarn](https://yarnpkg.com/)
- [Docker](https://www.docker.com/) (opcional, para ejecución con contenedores)

---

## 🚀 Instalación y ejecución

### 🔹 Opción 1: Ejecutar en local (sin Docker)

1. Clona el repositorio con sus submódulos:
   ```sh
   git clone --recurse-submodules https://github.com/Alexbyte95/testOrbi.git
   cd testOrbi

cd service-a && npm install && cd ..

cd service-b && npm install

cd service-a && npm run start

cd service-b && npm run start


🔹 Opción 2: Ejecutar con Docker

Asegúrate de estar en la raíz del proyecto y construye los contenedores:


docker-compose up --build
Los servicios estarán corriendo automáticamente.

Para detener los contenedores:

docker-compose down

Documentación
Cada servicio expone su documentación en Swagger:

Service A: http://localhost:3000/api
Service B: http://localhost:4000/api


🛠 Herramientas y Tecnologías
Node.js 20+
TypeScript
NestJS
gRPC (@grpc/grpc-js)
RabbitMQ
Docker & Docker Compose
OpenAPI/Swagger
Protobuf
