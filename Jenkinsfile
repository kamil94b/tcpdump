pipeline {
  agent any
  stages {
    stage('Build') {
      agent {
        docker {
          image 'ubuntu'
          args '-u 0'
        }

      }
      steps {
        sh '''id
env
pwd'''
        sh 'sudo apt install gcc'
        sh './configure'
      }
    }
  }
}