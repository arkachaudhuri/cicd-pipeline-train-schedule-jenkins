pipeline {
  agent any
  stages {
    stage ('Build') {
      steps {
        echo "Running pipeline build"
        sh "./gradlew build --no-daemon"
        archiveArtifact artifact: 'dist/trainSchedule.zip'
      }
    }
  }
}
