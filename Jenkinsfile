pipeline {
  agent any

  tools {
    nodejs "Node-18" // defined in Jenkins global tool config
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
        sh './node_modules/.bin/mocha'
      }
    }
    stage('Deploy') {
      steps {
        echo 'Deploy step (simulated)'
      }
    }
  }
}
