pipeline {
  agent any
  stages {
    stage('BUZZ BUZZ') {
      steps {
        echo 'Step 1'
        sh 'touch filetest.ttxt'
      }
    }

    stage('Bees Bees') {
      steps {
        echo 'Buzz, Bees, Buzz!'
        echo 'Bees Buzzing!'
        sh 'echo "yew yew"'
        sh 'mv filetest.ttxt filetestt.txt'
      }
    }

    stage('manual input') {
      steps {
        input(message: 'hi, input please', ok: 'go')
        sh 'ping 172.20.10.3'
      }
    }

  }
}