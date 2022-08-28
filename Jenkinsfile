pipeline {
    agent any
    stages {
        stage('Update the yaml file') {
            steps {
                script {
//                     sh 'echo ${params.Version}'                  
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
                        println conf.packages[23].versions[0]
                        r = conf.packages[23].versions[0]
                        
                        def matcher = r =~ /^1.3.0\-build.(?<minor>\d.*)$/
                        matcher.matches() 
                        minor-version = matcher.group("minor")
                        Integer current-minor-version = minor-version as Integer
                        println current-minor-version
                        
                    }
                }
            }
        }
    }
}
