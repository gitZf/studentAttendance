pipeline {
    agent any

    stages {
        stage('Build') {
            steps {
                echo 'Building..'
                git 'https://github.com/gitZf/studentAttendance.git
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
