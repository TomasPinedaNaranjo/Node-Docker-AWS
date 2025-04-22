1. Configurar tu aplicación Node.js
Asegúrate de que tu archivo index.js esté configurado correctamente para que la aplicación escuche en todas las interfaces (0.0.0.0) y en el puerto que deseas (en este caso, el puerto 80).
Nota: Se debe habilitar la regla de seguridad en AWS

2. Crear un Dockerfile

3. Nos vamos a la instancia y hacemos pull del repositorio

4. Construir la imagen de Docker : sudo docker build -t node-app .

5. Subir la imagen a un contenedor en AWS EC2:  sudo docker run -d -p 8080:80 --name node-container node-app

6. Acceder a la aplicación desde el navegador: http://<tu-ip-publica>:8080
