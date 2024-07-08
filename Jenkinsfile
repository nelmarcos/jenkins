pipeline {
  agent any
  stages {
    stage('Buzz Build') {
      steps {
        sh '''pwd
./jenkins/build.sh'''
      }
    }

    stage('Buzz Archive') {
      steps {
        archiveArtifacts(artifacts: './jenkins/*.gz', fingerprint: true)
      }
    }

  }
}
