pipeline {
  agent any
  stages {
    stage('BUZZ BUILD') {
      steps {
        sh 'git pull'
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