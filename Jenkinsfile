pipeline {
  agent any
  stages {
    stage ('Build'){
      steps{
        echo 'Running Build automation'
        sh './gradlew buld --no-daemon'
        archiveArtifacts artifacts: 'dist/trainSchedule.zip'
      }
    }
  }
}
