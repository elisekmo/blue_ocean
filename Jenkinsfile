pipeline {
  agent {
    node {
      label 'docker'
    }

  }
  stages {
    stage('Test') {
      parallel {
        stage('Test') {
          steps {
            echo 'Testing'
          }
        }

        stage('Parallel') {
          steps {
            echo 'Running in parallel'
          }
        }

      }
    }

    stage('Build') {
      steps {
        echo 'Building'
      }
    }

    stage('Clean up') {
      steps {
        echo 'Cleaning'
      }
    }

  }
}