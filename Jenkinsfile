pipeline {
    agent any
    stages {
        stage('build') {
            steps {
                echo 'Python'
                sh 'cat Jenkinsfile'
                sh 'uname'
                sh 'yq to_entries 1.3.0.yaml'
            }
        }
    }
}
