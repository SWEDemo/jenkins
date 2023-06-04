pipeline {
    agent any

    stages {
        stage('Hello') {
            steps {
                cd C:\Users\L-106\Desktop\2023 소공\SeleniumExample
                mvn clean test
            }
        }
    }
    
    post {
        always {
            echo 'pipeline finished'
        }
    }
}
