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
        archiveArtifacts(artifacts: './jenkins/test.txt.gz', fingerprint: true)
      }
    }

  }
}
