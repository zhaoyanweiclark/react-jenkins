pipeline {
    agent {
        docker {
            image 'node:14.17' 
            args '-p 3000:3000' 
        }
    }
    environment {
        AWS_KEY     = credentials('AWS_KEY')
    }
    stages {
        stage('Build') { 
            steps {
                echo $AWS_KEY
            }
        }
    }
}
