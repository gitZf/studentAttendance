pipeline {
    agent any

    stages {
        stage('Fetch from GitHub') {
                steps {
                    echo 'Building..'
                    git 'https://github.com/gitZf/studentAttendance.git'
                }
            }
        stage('Build') {
            steps {
                echo 'Building..'
            }
        }
        stage('Test') {
            steps {
                echo 'Testing..'
                javac Student.java
            }
        }
        stage('Deploy') {
            steps {
                echo 'Deploying....'
            }
        }
    }
}
