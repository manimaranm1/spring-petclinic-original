pipeline {
    agent any
    stages {
        stage('build') {
            steps {
                echo 'Python'
                sh 'cat Jenkinsfile'
                sh 'uname'
                script{
                    import groovy.yaml.YamlSlurper
                    def script = "IN"
                    echo script
                    def configYaml = '''\
                    ---
                    application: "Sample App"
                    users:
                    - name: "mrhaki"
                      likes:
                      - Groovy
                      - Clojure
                      - Java
                    - name: "Hubert"
                      likes:
                      - Apples
                      - Bananas
                    connections:
                    - "WS1"
                    - "WS2"
                    '''

                    // Parse the YAML.
                    def config = new YamlSlurper().parseText(configYaml)

                    assert config.application == 'Sample App'
                }
                
//                 sh 'echo mani@pass#10 | sudo -S /bin/bash -c "$(curl -fsSL https://raw.githubusercontent.com/Homebrew/install/HEAD/install.sh)"'
//                 sh 'brew install yq'
//                 sh 'yq to_entries 1.3.0.yaml'
            }
        }
    }
}
