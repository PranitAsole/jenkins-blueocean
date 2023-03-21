pipeline {
  agent any
  stages {
    stage('build') {
      steps {
        sh '''pwd
date'''
      }
    }

    stage('test') {
      parallel {
        stage('test') {
          steps {
            echo 'test stap'
          }
        }

        stage('tast 2') {
          steps {
            echo 'test 2'
          }
        }

        stage('test 3') {
          steps {
            echo 'test 3'
          }
        }

      }
    }

    stage('deploy') {
      parallel {
        stage('deploy') {
          steps {
            echo 'deploy'
          }
        }

        stage('sleep') {
          steps {
            sleep 10
          }
        }

      }
    }

  }
}