pipeline {
  agent any
  stages {
    stage('build') {
      steps {
        sh 'echo Build is successful'
      }
    }

    stage('Test') {
      steps {
        sh 'echo Test is successful calling from ${JOB_NAME}'
      }
    }

    stage('stage') {
      steps {
        sh 'echo "Hii good morning 21225"'
      }
    }

  }
}