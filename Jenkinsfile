pipeline {
  agent any
  stages {
    stage('BUZZ BUILD') {
      steps {
        sh 'ping 192.168.1.87'
        sh 'git pull'
        sh "chmod +x -R ${env.WORKSPACE}"
        sh './build.sh'
        archiveArtifacts(artifacts: 'target/*.jar', fingerprint: true)
      }
    }

    stage('Buzz test') {
      steps {
        sh 'sleep 5'
        sh './test-all.sh'
      }
    }

  }
}