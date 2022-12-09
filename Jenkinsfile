pipeline {
    agent any

       stages {
        
        stage('Dockerbuild') {
            steps {
                
               sh "docker build -t jatinsingh2604/javaprogramapp:2 ."

                }
                        }
        stage('Dockerlogin') {
            steps {
                
                sh "docker login" 

                }
                                }
        stage('Dockerpush') {
            steps {
                
                sh "docker push jatinsingh2604/javaprogramapp:2" 

                }
                            }
                

            
            }
        }
    


