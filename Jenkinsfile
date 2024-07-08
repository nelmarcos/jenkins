pipeline {
  agent any
  stages {
    stage('Buzz Build') {
      steps {
        sh './jenkins/build.sh'
        archiveArtifacts(artifacts: 'jenkins/*.gz', fingerprint: true)
      }
    }

    stage('Buzz Archive') {
      steps {
        sh 'pwd'
      }
    }

  }
}
