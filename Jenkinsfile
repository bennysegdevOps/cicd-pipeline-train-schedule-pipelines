pipeline {
  agent any
  stages {
    stage ('Build the process) {
      steps {
        echo 'Running build automation'
        ssh './gradlew build --no-daemon'
        archiveArtifacts artifacts: 'dist/trainSchedule.zip'
      }
    }
  }
}
