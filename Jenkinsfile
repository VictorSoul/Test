pipeline {
    agent any

    stages {
        stage('Build') {
            steps {
               sh  'mvn clean package'
            }
        }
        stage('Test') {
            steps {
               sh 'docker cp target/test-0.0.1-SNAPSHOT.war test2:/opt/apache-tomcat-9.0.1/webapps/tese.war'
            }
        }
        stage('Deploy') {
            steps {
                echo 'Deploying....1'
            }
        }
    }
}