pipeline {
  agent any
  stages {
    stage('Dev') {
      steps {
        echo 'I want to print'
      }
    }

    stage('Test') {
      parallel {
        stage('Test') {
          steps {
            echo 'I want to print'
          }
        }

        stage('Deploy') {
          steps {
            echo 'I want to deploy'
          }
        }

      }
    }

  }
}