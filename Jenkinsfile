pipeline {
    agent any
    stages {
        stage('build') {
            steps {
                echo 'Python'
                sh 'cat Jenkinsfile'
                sh 'yq -i '.packages.name |= test' 1.3.0.yaml'
            }
        }
    }
}
