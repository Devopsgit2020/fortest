pipeline {
  agent any
  stages {
    stage('BUZZ BUILD') {
      when {
        environment name: 'name', value: 'yassine'
      }
      steps {
        sh 'ping -c 5 192.168.1.87'
        sh 'git pull'
        sh "chmod +x -R ${env.WORKSPACE}"
        sh './build.sh'
        archiveArtifacts(artifacts: 'target/*.jar', fingerprint: true)
      }
    }

    stage('Buzz test') {
      when {
        branch 'simple-pipelin'
      }
      steps {
        sh 'sleep 5'
        sh "chmod +x -R ${env.WORKSPACE}"
        sh './test-all.sh'
      }
    }

  }
  environment {
    name = 'yassine'
  }
}