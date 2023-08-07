pipeline {
    agent any
    stages {
        stage('Build Docker Image') {
            steps {
                script {
                    def image = docker.build('my-docker-image')
                    echo "Docker image built: ${image.id}"
                }
            }
        }
        stage('Run Docker Container') {
            steps {
                script {
                    def container = docker.image('my-docker-image').run('-p 8081:80')
                    echo "Docker container started: ${container.id}"
                }
            }
        }
    }
}
