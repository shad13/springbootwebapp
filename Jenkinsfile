pipeline {
  agent any

    stages {
    stage('Build') {
      steps {
        sh "mvn package"
      }
    }
    
    stage('Make Container') {
      steps {
      sh "docker build -t springg1 ."
      sh "docker tag springg1 springg1:latest"
      }
    }
  }
}
