pipeline {
  agent any
  stages {
    stage('development') {
      steps {
        echo 'this is development'
      }
    }

    stage('Test') {
      steps {
        echo 'Tsting'
        echo 'This is build'
      }
    }

    stage('Build') {
      parallel {
        stage('Build') {
          steps {
            echo 'HUHUu'
          }
        }

        stage('fixes') {
          steps {
            echo 'fixes'
          }
        }

        stage('Operate') {
          steps {
            echo 'Operate'
          }
        }

        stage('Prod') {
          steps {
            echo 'Prod'
          }
        }

        stage('Deploy') {
          steps {
            echo 'Deploy'
          }
        }

      }
    }

  }
}