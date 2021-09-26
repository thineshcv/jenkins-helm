pipeline {
    agent any

    stages {
        stage('Build') {
            steps {
                echo 'Building..'
		 checkout scm
		 def customImage = docker.build("reactfe:${env.BUILD_ID}")
		 customImage.push()
            }
        }
        stage('Test') {
            steps {
                echo 'Testing..'
            }
        }
        stage('Deploy') {
            steps {
                echo 'Deploying....'
            }
        }
    }
}
