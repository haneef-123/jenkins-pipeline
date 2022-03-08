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
            echo "testing application ${ChromeDriverPath}"
          }
        }

      }
    }

    stage('deploy') {
      steps {
        echo 'deploy print'
        input(message: 'Do you want to deploy', id: 'Ok')
      }
    }

  }
  environment {
    ChromeDriverPath = '/Users/haneef/Downloads/'
  }
}