pipeline {
    agent {
        label {demoAgent}
    }

    stages {
        stage('Selenium Test') {
            steps {
                git branch: 'main ', poll: false, url: 'https://github.com/SWEDemo/jenkins.git'
                bat 'mvn clean test'
            }
        }
    }
}
