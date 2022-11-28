pipeline {
    agent any

       stages {
        stage('Build') {
            steps {
                
                sh "git 'https://github.com/jatin2604/DockerAssign'"

                }
        stage('Dockerbuild') {
            steps {
                
               sh "docker build -t jatinsingh2604/javaprog:1 ."

                }
        stage('Dockerlogin') {
            steps {
                
                sh "docker login" 

                }
        stage('Dockerpush') {
            steps {
                
                sh "docker push javaprog:1" 

                }
                

            
            }
        }
    }
}

