pipeline {
    agent any

    stages {
        stage('Hello') {
            steps {
                echo 'Hello Hongik'
            }
        }
    }
    
    post {
        always {
            echo 'pipeline finished'
        }
    }
}
