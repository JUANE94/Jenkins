# Jenkins
#Crear imagen
cd jenkinsdocker
docker build -t jenkins-cicd --no-cache
#Correr contenedor
docker run -d -p 8080:8080 -p 5000:5000 --name jenkins jenkins-cicd
