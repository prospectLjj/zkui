pipeline {
  agent any
  stages {
    stage('') {
      steps {
        sh '''cd zkui
mvn clean install 
ll target/zkui-2.0-SNAPSHOT-jar-with-dependencies.jar'''
      }
    }

  }
}