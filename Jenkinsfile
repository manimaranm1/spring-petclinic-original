pipeline {
    agent any
    stages {
        stage('Update the yaml file') {
            steps {
                script {
                    def conf = readYaml file: "1.3.0.yaml"
                    def st = conf.toString()
                    echo st
                    echo conf.packages.toString()
//                     echo conf.packages.[0].toString()
                    println conf.getClass()
                    println st.getClass()
                    println conf
                    println conf.packages.name[23]
                    if (conf.packages[23].name == 'tap') {
                        println conf.packages.versions[23]
                        println conf.packages[23].versions
                    }
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
