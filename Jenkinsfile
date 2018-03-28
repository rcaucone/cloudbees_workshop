pipeline {
  agent any
  stages {
    stage('My Test Stage') {
      steps {
        sh 'printenv > env.txt'
      }
    }
    stage('Archive') {
      steps {
        archiveArtifacts 'env.txt'
      }
    }
    stage('Sleep 10 seconds') {
      steps {
        sleep 10
      }
    }
  }
}