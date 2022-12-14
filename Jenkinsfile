pipeline {
    agent any

    stages {

        stage('Clean') {
            steps {
              powershell.exe -Command "mvn clean"
            }
        }

        stage('Test') {
            steps {
              powershell.exe -Command "mvn test"
            }
        }

        stage('Deploy') {
            steps {
              powershell.exe -Command "mvn package"
              }
        }

    }
}
