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
        junit '/var/jenkins_home/workspace/jenkins_simple-pipeline/jenkins/jacocoTestReport.xml'
      }
    }

  }
}
