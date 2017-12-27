pipeline {
    agent any

    stages {
        stage('Build') {
            steps {
                echo 'Building..'
                git 'https://github.com/gitZf/studentAttendance.git'
                sh 'javac studentAttendance/Student.java'
                sh 'javac -cp ../junit-4.12.jar:. studentTest.java'
               
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
