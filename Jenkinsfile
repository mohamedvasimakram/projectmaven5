pipeline{
  agent 
  {
    label 'java_slave_node'
  }
  tools
  {
    maven 'maven'
  stages{
    stage("print server info"){
      steps{
        sh 'mvn clean package'
      }
    }
  }
}
