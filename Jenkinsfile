
pipeline {
  agent any
  stages {
    stage ("git clone") {
      steps {
        git clone r
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
