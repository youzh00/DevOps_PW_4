pipeline {
    agent any

    stages {

        stage('Clean') {
            steps {
              set path=%path%;C:\\Program Files\\apache-maven-3.8.6\\bin
              mvn clean
            }
        }

        stage('Test') {
            steps {
              bat "set path=%path%;C:\\Program Files\\apache-maven-3.8.6\\bin"
              bat "mvn test"
            }
        }

        stage('Deploy') {
            steps {
              bat "set path=%path%;C:\\Program Files\\apache-maven-3.8.6\\bin"
              bat "mvn package"
              }
        }

    }
}
