pipeline {
  agent any
  stages {
    stage('Upload to AWS') {
      steps {
        withAWS(credentials:'aws-static')
          {
            s3Upload(file:'index.html', bucket:'ud-devops-project4-bucket1', path:'/')
          }
      }
    }
  }
}
