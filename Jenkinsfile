pipeline {
    agent any

    stages {

        stage('Env') {
            steps {
              bat "set path=%path%;C:\\Program Files\\apache-maven-3.8.6\\bin"
            }
        }
        stage('Clean') {
            steps {
              bat "set path=%path%;C:\\Program Files\\apache-maven-3.8.6\\bin && mvn clean"
            }
        }

        stage('Test') {
            steps {
              bat "set path=%path%;C:\\Program Files\\apache-maven-3.8.6\\bin && mvn test"
            }
        }

        stage('Deploy') {
            steps {
              bat "set path=%path%;C:\\Program Files\\apache-maven-3.8.6\\bin && mvn package"
              }
        }

    }
}
