pipeline {
    agent any

    stages {
        stage('Checkout') {
            steps {
                #git 'https://github.com/Kwasi200/retail-app.git'
                git branch: 'main', url: 'https://github.com/Kwasi200/retail-app.git'
            }
        }

        stage('Build') {
            steps {
                sh 'mvn clean package'
            }
        }
    }
}
