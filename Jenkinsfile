pipeline {
    agent any

    stages {
        stage('Build') {
            steps {
                echo 'Building..'
                git 'https://github.com/gitZf/studentAttendance.git'
                //sh 'javac studentAttendance/Student.java'
                sh 'javac -cp junit-4.12.jar:. studentAttendance/Student.java studentAttendance/studentTest.java'
                sh 'java -cp junit-4.12.jar:hamcrest-core-1.3.jar:. org.junit.runner.JUnitCore studentAttendance/studentTest'
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
