# Crea el archivo con este contenido básico
echo 'pipeline {
    agent any
    stages {
        stage("Build") {
            steps {
                sh "docker build -t eva2-app ."
            }
        }
        stage("Run") {
            steps {
                sh "docker run -d -p 9999:9999 --name eva2-container eva2-app"
            }
        }
    }
}' > Jenkinsfile