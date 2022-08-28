pipeline {
    agent any
    stages {
        stage('build') {
            steps {
                echo 'Python'
                sh 'cat Jenkinsfile'
                sh 'uname'
                script {
                    def conf = readYaml file: "1.3.0.yaml"
                    assert conf.packages.name == "cert-manager"
                }
            }
                
//                 sh 'echo mani@pass#10 | sudo -S /bin/bash -c "$(curl -fsSL https://raw.githubusercontent.com/Homebrew/install/HEAD/install.sh)"'
//                 sh 'brew install yq'
//                 sh 'yq to_entries 1.3.0.yaml'
//             }
        }
    }
}
