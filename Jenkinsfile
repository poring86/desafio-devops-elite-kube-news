pipeline{
  agent any

  stages{
    stage('Build Docker Image'){
      steps{
        script{
          dockerapp = docker.build("poring86/kube-news", '-f ./src/Dockerfile ./src')
        }
      }
    }
  }
}