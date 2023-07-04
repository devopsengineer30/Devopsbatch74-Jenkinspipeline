pipeline {
  agent any
  stages {
    stage('dev') {
      steps {
        echo 'this is development'
      }
    }

    stage('Test') {
      steps {
        echo 'This is test stage'
      }
    }

    stage('build') {
      parallel {
        stage('build') {
          steps {
            echo 'this is build'
          }
        }

        stage('fixes') {
          steps {
            echo 'This is fixes stage'
          }
        }

        stage('Operate') {
          steps {
            echo 'This is operate'
          }
        }

        stage('Prod') {
          steps {
            echo 'This is Prod'
          }
        }

        stage('Deploy') {
          steps {
            echo 'This is deployment'
          }
        }

      }
    }

  }
}