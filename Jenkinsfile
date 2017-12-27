pipeline {
    agent any

    stages {
        stage('Build') {
            steps {
                echo 'Building..'
                sh 'javac Student.java'
            }
        }
        stage('Test') {
            steps {
                echo 'Testing..'
                //sh javac Student.java
            }
        }
        stage('Deploy') {
            steps {
                echo 'Deploying....'
                //sh
            }
        }
        
        //post {
        //    always {
        //        junit '*.xml'
        //    }
        //} 
    }
}
