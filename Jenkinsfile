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
               sh 'docker copy targrt/test-0.0.1-SNAPSHOT.war test1:/opt/apache-tomcat-9.0.1/webapps/tese.war'
            }
        }
        stage('Deploy') {
            steps {
                echo 'Deploying....1'
            }
        }
    }
}