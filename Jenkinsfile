
pipeline {
  agent any
  stages {
    stage ("git clone") {
      steps {
        git url
      }
    }
    stage ("maven build") {
      steps {
        mvn clean
      }
    }
    stage ("sonar codeanalysis") {
     steps {
       sonarqube
     }
    }
  }
}
