pipeline {
  agent any
  stages {
    stage('Build') {
      steps {
        echo 'Build app 2!'
        writeFile file: "application.sh", text: "echo Built ${BUILD_ID} of ${JOB_NAME}"
        archiveArtifacts artifacts: '*.sh', fingerprint: true
      }
    }
  }
}
