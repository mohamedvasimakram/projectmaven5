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
               sh '''
               docker stop hello || true
               docker rm -rf hello || true
               docker run -it -d --name hello -p 80:80 nginx
               '''
            }
        }
     }
}
