pipeline {
  agent any
  stages {
    stage ('Build') {
      steps {
        echo 'Running build automation'
        sh './gradlew build --no-daemon'
        archiveArtifacts artifacts: 'dist/trainSchedule.zip'
       }
      stage ('echo out something') {
      steps {
        echo 'Checking for echo'
       }
     }
  }
}
