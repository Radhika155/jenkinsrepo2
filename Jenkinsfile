pipeline {
  agent any
  stages {
    stage('Build') {
      steps {
        echo 'Build started'
      }
    }

    stage('Dev') {
      parallel {
        stage('Dev') {
          steps {
            echo 'Dev environment'
          }
        }

        stage('QA') {
          steps {
            echo 'QA Environement'
          }
        }

      }
    }

    stage('PROD') {
      steps {
        echo 'PROD Environment'
      }
    }

  }
}