pipeline {
    agent any

    checkout([$class: 'GitSCM', branches: [[name: '*/master']], extensions: [], userRemoteConfigs: [[url: 'https://github.com/jatin2604/DockerAssign.git']]])
       stages {
        
        stage('Dockerbuild') {
            steps {
                
               sh "docker build -t jatinsingh2604/javaprogram:2 ."

                }
                        }
        stage('Dockerlogin') {
            steps {
                
                sh "docker login" 

                }
                                }
        stage('Dockerpush') {
            steps {
                
                sh "docker push jatinsingh2604/javaprogram:2" 

                }
                            }
                

            
            }
        }
    


