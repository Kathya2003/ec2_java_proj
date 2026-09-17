pipeline {
    agent any
    stages {
        stage('compile') {
            steps {
                sh 'javac Program1.java'
            }
        }
        stage('run') {
            steps {
                sh 'java Program1'
            }
        }
        stage('email') {
            steps {
                emailext body: 'java project is executed', 
                         subject: 'generating mail for java proj', 
                         to: 'ramapuram2003@gmail.com'
            }
        }
    }
}
