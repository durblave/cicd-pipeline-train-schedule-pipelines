pipeline {
  agent any
  stages {
    stage ("build") {
      steps {
        echo "######################### Running Build Automation #########################"
        sh "./gradle build --no-daemon"
        archiveArtifacts artifacts: "dist/trainSchedule.zip"
      }
    }
  }
}
