pipeline
{
    agent any
    stages
    {
        stage('nginx image')
        {
            steps
            {
                sh 'docker pull nginx'
            }
        }
    stage('run container')
    {
        steps
        {
            sh 'docker run -it -d --name app -p 80:81 nginx'
        }
    }
    }
}
