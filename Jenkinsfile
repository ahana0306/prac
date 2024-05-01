pipeline {
    agent any

    stages {
        stage('Checkout') {
            steps {
                git branch: 'main', url: 'https://github.com/ahana0306/prac.git'
            }
        }
        
        stage('Build') {
            steps {
                echo 'Building...'
            }
        }
        
        stage('Deploy') {
            steps {
                echo 'Deploying...'
                bat "xcopy /Y /I /E /F /C *.html C:\\xampp\\htdocs\\"
            }
        }
    }
}

     
