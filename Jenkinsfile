pipeline{
    agent any
    stages {
        stage('nginx image'){
            steps{
                sh 'docker pull nginx'
            }
         }
        stage('to run container'){
            steps{
               sh 'docker stop hello || true'
               sh 'docker rm -rf hello || true'
               sh 'docker run -it -d --name hello -p 8081:8000 nginx'
            }
        }
     }
}
