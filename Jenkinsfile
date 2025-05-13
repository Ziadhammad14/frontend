pipeline {
  agent any
  tools {
    gradle 'gradle'
  }
  stages {
    stage("run frontend") {
      steps {
        echo 'executing yarn...'
        nodejs('NodeJS') {
          sh 'yarn install'
        }
      }
    }
    stage("run backend") {
      steps {
        echo 'executing gradle...'
          sh './gradlew -v'
        
      }
    }
  }
}
