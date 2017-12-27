pipeline {
    agent any

    stages {
        stage('Build') {
            steps {
                echo 'Building..'
                git 'https://github.com/gitZf/studentAttendance.git'
                //sh 'javac studentAttendance/Student.java'
                sh 'javac -cp junit-4.12.jar:. studentAttendance/Student.java studentAttendance/studentTest.java'
                
            }
        }
        stage('Test') {
            steps {
                echo 'Testing..'
                sh 'java -cp junit-4.12.jar:hamcrest-core-1.3.jar:. org.junit.runner.JUnitCore /var/lib/jenkins/workspace/Student Test/studentAttendance/studentTest'
            }
        }
        stage('Deploy') {
            steps {
                echo 'Deploying....'
                
            }
        }
        
    }
}
