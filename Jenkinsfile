pipeline {
    agent any
    parameters {
        string(name: 'cert-manager', defaultValue: '', description: 'Enter')
    }
    stages {
        stage('Read the yaml file tap version') {
            steps {
                script {    
                    echo "Hello ${params.cert-manager}"
//                     def conf = readYaml file: "repos/1.3.0.yaml"
//                     def st = conf.toString()
//                     echo st
//                     echo conf.packages.toString()

//                     println conf.getClass()
//                     println st.getClass()
//                     println conf
//                     println conf.packages.name[23]
//                     if (conf.packages[23].name == 'tap') {
//                         println conf.packages.versions[23]
//                         println conf.packages[23].versions[0]
//                         r = conf.packages[23].versions[0]
                        
//                         def matcher = r =~ /^1.3.0\-build.(?<minor>\d.*)$/
//                         matcher.matches() 
//                         minor_version = matcher.group("minor")
//                         Integer current_minor_version = minor_version as Integer
//                         println current_minor_version
//                         new_minor_version = "1.3.0-build." + (current_minor_version + 1)
//                         println new_minor_version
                        
                    }
                }
            }
        }
//         stage('Update the yaml file tap version') {
//             steps {
//                 script {                
//                     def conf = readYaml file: "1.3.0.yaml"
//                     conf.packages[23].versions[0] = conf.packages[23].versions[0].replaceFirst(r,new_minor_version)
//                     println conf.packages[23].versions[0]
//                     println conf
// //                     sh 'git clone https://github.com/manimaranm1/spring-petclinic-original.git'
//                     sh 'git checkout main'
//                     sh 'git pull'
//                     writeYaml file: '1.3.0.yaml', data:conf, overwrite:true
//                     println "After"
//                     println conf
//                     def conf2 = readYaml file: "1.3.0.yaml"
//                     println conf
//                     sh 'git config --global user.name "manimaranm1"'
//                     sh 'git config --global user.name'
//                     sh 'git status'
//                     sh 'git add 1.3.0.yaml'
//                     sh 'git commit -m "changes for 1.3.0-build.14"'
// //                     sh 'git remote add origin git@github.com:manimaranm1/spring-petclinic-original.git'
//                     sh 'git remote -v'
// //                     sh 'ssh -T git@github.com'
//                     sh 'git push origin --all'
//                 }
//             }
//         }

    }
}
