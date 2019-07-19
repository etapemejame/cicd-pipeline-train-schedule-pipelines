pipeline {
  agent any
  statges {
    stage ('Build') {
      steps {
        echo 'Running build automation'
        sh './gradlew build --no-deamon'
        archiveArtifacts artifacts: 'dist/trainSchedule.zip'
      }
    }
  }
}
