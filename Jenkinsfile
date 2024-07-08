pipeline {
  agent any
  stages {
    stage('Buzz Build') {
      steps {
        sh './jenkins/build.sh'
      }
    }

    stage('Buzz Archive') {
      steps {
        sh 'pwd'
        archiveArtifacts(artifacts: './jenkins/test.txt.gz', fingerprint: true)
      }
    }

  }
}
