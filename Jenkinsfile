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
        archiveArtifacts 'filetestt.txt'
      }
    }

  }
}