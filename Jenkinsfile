pipeline {
    agent any
    stages {
        stage('build') {
            steps {
                echo 'Python'
                sh 'cat Jenkinsfile'
                sh 'uname'
                sh '/bin/bash -c "$(curl -fsSL https://raw.githubusercontent.com/Homebrew/install/HEAD/install.sh)"'
                sh 'brew install yq'
                sh 'yq to_entries 1.3.0.yaml'
            }
        }
    }
}
