# despliegue-todo-davidbaquero
# despliegue-todo-davidbaquero
Este proyecto corresponde a una aplicación Full Stack orientada a la administración de tareas. Permite crear, visualizar, actualizar, marcar como finalizadas y eliminar tareas según sea necesario.
El backend está desarrollado con Node.js y Express, utilizando PostgreSQL como base de datos alojada en Railway.

Tecnologías

Backend: Node.js, Express, CORS, Dotenv, PostgreSQL
Base de Datos: PostgreSQL (Railway)
Frontend (en desarrollo): HTML, CSS, JavaScript o React
Control de Versiones: Git
Despliegue: Railway

Variables de Entorno (Railway / .env.local)

Para ejecutar el proyecto correctamente se deben definir las siguientes variables:

DB_HOST=tramway.proxy.rlwy.net
DB_USER=root
DB_PASSWORD=AXTxLbdYRDhKbCjCcGiuiLkjuWwmuglD
DB_NAME=railway
DB_PORT=35810

Endpoints de la API
Método	Ruta	Descripción
GET	/tasks	Obtiene todas las tareas
POST	/tasks	Crea una tarea nueva
PUT	/tasks/:id/complete	Marca una tarea como completada
DELETE	/tasks/:id	Elimina una tarea

Ejemplo de respuesta JSON:

{
  "id": 1,
  "title": "Tarea de ejemplo",
  "completed": false
}

Ejecución del Backend en Local

Clonar el repositorio:

git clone <URL-de-tu-repo>
cd backend


Instalar dependencias:

npm install


Crear el archivo .env.local con las variables de entorno indicadas.

Iniciar el servidor:

npm run dev

Despliegue en Railway

El proyecto está configurado para funcionar automáticamente al conectar el repositorio y establecer las variables de entorno en Railway. Una vez configurado esto, Railway gestiona el despliegue.

Próximas tareas

Finalizar la interfaz del frontend

Establecer comunicación entre frontend y backend

Mejorar estilos mediante CSS o algún framework

Información

Este proyecto se realizó como ejercicio de práctica para fortalecer habilidades en desarrollo Full Stack y despliegue en la nube.
