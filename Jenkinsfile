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
                    def st = conf.toString()
                    echo st
                    echo conf.packages.toString()
//                     echo conf.packages.[0].toString()
                    println conf.getClass()
                    println st.getClass()
                    println conf.packages
//                     echo st.getClass()
                   
                }
            }
                
//                 sh 'echo mani@pass#10 | sudo -S /bin/bash -c "$(curl -fsSL https://raw.githubusercontent.com/Homebrew/install/HEAD/install.sh)"'
//                 sh 'brew install yq'
//                 sh 'yq to_entries 1.3.0.yaml'
//             }
        }
    }
}
