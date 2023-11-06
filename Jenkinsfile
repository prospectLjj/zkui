pipeline {
  agent any
  stages {
    stage('error') {
      steps {
        dir(path: '/var/jenkins_home/workspace/zkui_master') {
          sh '''/var/jenkins_home/maven/apache-maven-3.9.5/bin/mvn clean package install
ls -lh target/zkui-2.0-SNAPSHOT-jar-with-dependencies.jar
'''
        }

      }
    }

  }
}