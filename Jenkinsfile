pipeline {
  agent any

  tools {
    nodejs "NodeJS" // defined in Jenkins global tool config
  }

  stages {
    stage('Clone') {
      steps {
        git 'https://github.com/Chocomimin/hello-jenkins'
      }
    }
    stage('Install') {
      steps {
        sh 'npm install'
      }
    }
    stage('Test') {
      steps {
        sh 'npm test'
      }
    }
    stage('Deploy') {
      steps {
        echo 'Deploy step (simulated)'
      }
    }
  }
}
