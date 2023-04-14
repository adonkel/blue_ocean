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
            echo '"testing"'
          }
        }

        stage('Parallel') {
          steps {
            echo 'Parallel running'
          }
        }

      }
    }

    stage('Build') {
      steps {
        echo 'building'
      }
    }

    stage('Clean Up') {
      steps {
        echo 'Clean Env'
      }
    }

  }
}