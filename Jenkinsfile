pipeline {
    agent any
    stages {
        stage('git') {
            steps {
                // Get some code from a GitHub repository
                git branch: 'main', url: 'https://github.com/SWEDemo/jenkins.git'
            }
        }        
        stage('mvn') {
            steps {
                // Run Maven on a Window agent.
                bat "mvn -Dmaven.test.failure.ignore=true clean test"
            }
        }
    }
}
