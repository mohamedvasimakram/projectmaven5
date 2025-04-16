pipeline{
  agent any 
  stages{
    stage("print server info"){
      steps{
        sh """
        echo ${env.JOB_NAME}
        echo ${env.BULID_ID}
        uptime
        whoami
        pwd
        echo ${env.HOSTNAME}
        """
      }
    }
  }
}
