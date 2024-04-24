
pipeline {
  agent any
  stages {
    stage ("git clone") {
      steps {
        git clone repourl
      }
    }
    stage ("maven build") {
      steps {
        mvn clean
      }
    }
  }
}
