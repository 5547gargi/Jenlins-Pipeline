pipeline {
  agent any
  stages {
    stage('dev') {
      steps {
        echo 'dev state'
      }
    }

    stage('test') {
      steps {
        echo 'testing stage'
      }
    }

    stage('build') {
      parallel {
        stage('build') {
          steps {
            echo 'build stage'
          }
        }

        stage('fix') {
          steps {
            echo 'fix stage'
          }
        }

        stage('operation') {
          steps {
            echo 'this is operation'
          }
        }

        stage('prod') {
          steps {
            echo 'productionstage'
          }
        }

        stage('deploy') {
          steps {
            echo 'deployment stage'
          }
        }

      }
    }

  }
}