pipeline {
  agent any
  stages {
    stage('BUZZ BUZZ') {
      parallel {
        stage('BUZZ BUZZ') {
          steps {
            echo 'Step 1'
          }
        }

        stage('test buzz parallel') {
          steps {
            echo 'hi parallel'
          }
        }

      }
    }

  }
}