pipeline {
  agent any
  stages {
    stage('Checkout') {
      steps {
        echo 'Checking Out'
      }
    }

    stage('Build') {
      steps {
        echo 'Building'
      }
    }

    stage('Test1') {
      parallel {
        stage('Test1') {
          steps {
            echo 'Test1'
          }
        }

        stage('Test2') {
          steps {
            echo 'Test2'
          }
        }

      }
    }

    stage('Publish') {
      steps {
        echo 'Publishing'
      }
    }

  }
}