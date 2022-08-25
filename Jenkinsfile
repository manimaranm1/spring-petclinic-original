pipeline {
    agent any
    stages {
        stage('build') {
            steps {
                echo 'Python'
                sh 'cat Jenkinsfile'
                sh 'yq '.packages.name' 1.3.0.yaml'
            }
        }
    }
}
