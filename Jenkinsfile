flag = true
pipeline {
  agent any
  environment {
    NEW_VERSION = '1.3.0'
  }
  stages {
    stage('Build') {
    steps {
      echo 'Building..'
      // Here you can define commands for your build
      echo 'building version ${NEW_VERSION}'
    }
    }
    stage('Test') {
      steps {
        echo 'Testing..'
        // Here you can define commands for your tests
        }
    }
    stage('Deploy') {
      steps {
        echo 'Deploying....'
        // Here you can define commands for your deployment
      }
    }
  }
  post {
  always {
    echo 'post build condition running'
  }
  failure {
    echo 'post action if build failed'
  }
}

}
