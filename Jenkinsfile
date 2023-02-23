pipeline {
  agent any
  stages {
    stage('Dev') {
      steps {
        echo 'i want to develop'
      }
    }

    stage('Build') {
      parallel {
        stage('Build') {
          steps {
            echo 'i want to build'
          }
        }

        stage('Test') {
          steps {
            echo 'i want to test'
          }
        }

        stage('Deploy') {
          steps {
            echo 'i want to deploy'
          }
        }

      }
    }

  }
}