pipeline {
  agent any
  stages {
    stage('error') {
      steps {
        sh '''cd zkui_master
mvn clean install 
ll target/zkui-2.0-SNAPSHOT-jar-with-dependencies.jar'''
      }
    }

  }
}