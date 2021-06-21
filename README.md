# Tarea Docker
Aplicación Django conectada a una base de datos postgres.

# 1. Construir la imagen 
docker image build --tag=centro-comercial .

# 2. Subir la imagen a docker Hub
### 2.1 Primero hay que introducir las credenciales:
docker login

### 2.2 Etiqueto la imagen con mi usuario y el nombre de la imagen 
docker image tag centro-comercial adriangameromedina/centro-comercial

### 2.3 Subo la imagen al DockerHub
docker image push adriangameromedina/centro-comercial

# 3. Se puede probar la app con el docker-compose
docker-compose up -d

### 3.1 URL
http://localhost:8000

### Credenciales de la base de datos postgres
usuario: adrian
contraseña: admin1234
