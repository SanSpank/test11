pipeline {
  agent {

    docker {
      image '130.193.36.121:8123/builder:1.0.0'
    }

  }

  stages {

    stage('Build jar') {
      steps {
        git(url: 'https://github.com/SanSpank/test10.git', branch: 'master')
      }
    }
  }
}