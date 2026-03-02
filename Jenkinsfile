pipeline {
    agent any

    stages {
        stage('fetch file') {
            steps {
               git 'https://github.com/Pooja-2-5/jenkinsDemo.git'
            }
        }
         stage('Build') {
            steps {
                echo 'Building project'
                bat 'javac Hello.java'
            }
        }
         stage('executing') {
            steps {
                echo 'executing program'
                bat 'java Hello'
            }
        }
         stage('Devploy') {
            steps {
                echo 'deploying'
            }
        }
    }
    post{
        success{
            echo 'pipeline excuted successsfully'
        }
        failure{
            echo 'pipeline excuted fails'
        }
    
    }
}
