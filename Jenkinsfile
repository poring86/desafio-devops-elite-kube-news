pipeline{
  agent any

  stages{
    stage('Build Docker Image'){
      steps{
        script{
          dockerapp = docker.build("poring86/kube-news:${env.BUILD_ID}", '-f ./src/Dockerfile ./src')
        }
      }
    }
  }
}