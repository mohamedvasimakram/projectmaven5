pipeline{
    agent any
    stages {
        stage('nginx image'){
            steps {
                sh 'docker pull nginx'
            }
        }
        stage('to run container'){
            steps{
               sh'docker stop app5'
               sh'docker rm -rf app5'
               sh'docker run -it -d --name app5 -p 8081:80 nginx'
             }
        }
    }
}
