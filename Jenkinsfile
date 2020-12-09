pipeline {
  agent {

    docker {
      image '130.193.36.121:8123/builder:1.0.0'
    }

  }

  stages {

    stage('Git clone project') {
      steps {
        git(url: 'https://github.com/SanSpank/test10.git', branch: 'master')
      }
    }
    stage('Build war') {
      steps {
        sh 'mvn clean package'
        sh 'docker build -f test10/Dockerfile_app -t app_boxfuse:1.0.0 .'

      }
    }
  }
}