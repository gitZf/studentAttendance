pipeline {
    agent any

    stages {
        stage('Build') {
            steps {
                echo 'Building..'
                git 'https://github.com/gitZf/studentAttendance.git'

                sh 'cp studentAttendance/Student.java Student.java'
                sh 'cp studentAttendance/studentTest.java studentTest.java'
                
                sh 'javac -cp junit-4.12.jar:. Student.java studentTest.java'
                
                
            }
        }
        stage('Test') {
            steps {
                echo 'Testing..'
                sh 'java -cp junit-4.12.jar:hamcrest-core-1.3.jar:. org.junit.runner.JUnitCore studentTest'
            }
        }
        stage('Deploy') {
            steps {
                echo 'Deploying....'
                
            }
        }
        
    }
}
