pipeline {
    agent {
        docker {
            image 'node:14.17' 
            args '-p 3000:3000' 
        }
    }
    stages {
        stage('Build') { 
            steps {
                sh 'yarn' 
            }
        }
    }
}
