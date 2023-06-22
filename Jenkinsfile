pipeline {
  agent any
  stages {
    stage('BUZZ BUILD') {
      steps {
        echo "${env}"
        sh "chmod +x -R ${env.WORKSPACE}"
        sh './build.sh'
      }
    }

    stage('Buzz test') {
      steps {
        sh './test-all.sh'
      }
    }

  }
}