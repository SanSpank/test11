pipeline {
  agent {

    docker {
      image 'http://130.193.36.121:8123/builder:1.0.0'
    }

  }

  stages {

    stage('Build jar') {
      steps {
        sh 'mvn --version'
      }
    }
  }
}