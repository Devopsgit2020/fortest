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

    stage('test') {
      steps {
        tool(name: 'jdk8', type: 'jdk8')
      }
    }

  }
}