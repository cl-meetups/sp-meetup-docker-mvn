pipeline {
  agent any
  stages {
    stage('Preparacao') {
      steps {
        parallel(
          "Preparacao": {
            echo 'Hello World!'
            
          },
          "Passo Paralelo": {
            echo 'Executado em paralelo'
            sleep 5
            
          }
        )
      }
    }
    stage('Fortune') {
      steps {
        sh '/usr/games/fortune'
      }
    }
  }
}