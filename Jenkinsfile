pipeline {
  agent any
  stages {
    stage('Buzz Build') {
      steps {
        sh '''pwd
./jenkins/build.sh'''
      }
    }

    stage('Buzz Test') {
      steps {
        sh './jenkins/test-all.sh'
      }
    }

  }
}
