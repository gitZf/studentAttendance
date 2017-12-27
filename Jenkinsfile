pipeline {
    agent any

    stages {
        stage('Build') {
            steps {
                echo 'Building..'
                git 'https://github.com/gitZf/studentAttendance.git'
                sh 'javac studentAttendance/Student.java'
               
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
