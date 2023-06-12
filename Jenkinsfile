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
        sh '''sleep 10
echo Test is successful calling from ${JOB_NAME}'''
      }
    }

    stage('stage') {
      parallel {
        stage('stage') {
          steps {
            sh '''sleep 5
echo "Hii good morning 21225"'''
          }
        }

        stage('stage1.1') {
          steps {
            sh '''sleep 5
echo "This is parallel stage"'''
          }
        }

        stage('stage1.2') {
          steps {
            sh '''sleep 5
echo "Baby when you are coming"'''
          }
        }

        stage('stage1.3') {
          steps {
            sh '''sleep 5
echo "Baby come fast"'''
          }
        }

      }
    }

    stage('stage2') {
      steps {
        sleep 10
      }
    }

  }
}