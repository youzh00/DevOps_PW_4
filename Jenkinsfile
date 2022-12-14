pipeline {
    agent any
    stages {
        stage('Build') {
            steps {
                cmd.exe /C "set path=%path%;C:\Program Files\apache-maven-3.8.6\bin && mvn clean"
            }
        }
        stage('Test') {
            steps {
                cmd.exe /C "set path=%path%;C:\Program Files\apache-maven-3.8.6\bin && mvn test"
            }
        }
        stage('Deploy') {
            steps {
                cmd.exe /C "set path=%path%;C:\Program Files\apache-maven-3.8.6\bin && mvn package"
            }
        }
    }
}
