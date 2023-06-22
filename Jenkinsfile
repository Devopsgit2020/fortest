pipeline {
  agent any
  stages {
    stage('BUZZ BUILD') {
      steps {
        echo "${env.WORKSPACE}"
        sh "chmod +x -R ${env.WORKSPACE}"
        sh './build.sh'
      }
    }

  }
}