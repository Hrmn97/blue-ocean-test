pipeline {
  agent any
  stages {
    stage('Build') {
      steps {
        sh '''pwd
date
'''
      }
    }

    stage('Test Stage') {
      parallel {
        stage('Test Stage') {
          steps {
            echo 'Test step'
          }
        }

        stage('Test par') {
          steps {
            echo 'test par'
          }
        }

      }
    }

    stage('Deploy') {
      steps {
        echo 'Deploy'
        sleep 10
      }
    }

  }
}