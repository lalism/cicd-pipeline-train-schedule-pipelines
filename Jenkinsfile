pipeline {
  agent any
  stages {
    stage ('Build') { 
      steps {
        echo 'Running build automation'
        sh './gradlew build build --no-daemon'
        archiveArtifacts artifacts: 'dist/trainSchedule.zip'
      }
    }
  }
}
