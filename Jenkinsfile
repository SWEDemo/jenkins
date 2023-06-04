pipeline {
    agent {
        label 'demoAgent'
    }

    stages {
        stage('Selenium Test') {
            steps {
                git clean -f -d
                git clean -f -x
                git branch: 'main ', poll: false, url: 'https://github.com/SWEDemo/jenkins.git'
                bat 'mvn clean test'
            }
        }
    }
}
