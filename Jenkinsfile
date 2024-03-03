pipeline {
  agent any
  stages {
    stage('Build') {
      steps {
        sh '''pwd
date'''
      }
    }

    stage('test') {
      parallel {
        stage('test') {
          steps {
            echo 'test step'
          }
        }

        stage('test paralle') {
          steps {
            echo 'test running in paralle'
          }
        }

      }
    }

    stage('deploy') {
      steps {
        echo 'deploy stage'
        sleep 15
      }
    }

  }
}