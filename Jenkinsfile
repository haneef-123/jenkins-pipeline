pipeline {
  agent any
  stages {
    stage('Build') {
      parallel {
        stage('Build') {
          steps {
            echo 'this is test pipeline generator'
          }
        }

        stage('test') {
          steps {
            echo 'testing application'
          }
        }

      }
    }

    stage('deploy') {
      steps {
        echo 'deploy print'
      }
    }

  }
}