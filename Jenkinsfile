pipeline {
  agent any
  stages {
    stage('build') {
      steps {
        echo 'build stage'
      }
    }

    stage('test') {
      parallel {
        stage('test integration') {
          steps {
            echo 'test d\'int�gration'
          }
        }

        stage('test fonctionnel') {
          steps {
            echo 'test fonctionnel'
          }
        }

        stage('smoke') {
          steps {
            echo 'smoke test'
          }
        }

      }
    }

    stage('deploy') {
      steps {
        echo 'deploy'
      }
    }

  }
}