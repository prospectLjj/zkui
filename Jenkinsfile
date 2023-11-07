pipeline {
  agent any
  stages {
    stage('error') {
      steps {
        dir(path: '/var/jenkins_home/workspace/zkui_master') {
          sh '''echo "start build......"
/var/jenkins_home/maven/apache-maven-3.9.5/bin/mvn clean package install -Dmaven.repo.remote=http://maven.aliyun.com/nexus/content/groups/public
ls -lh target/zkui-2.0-SNAPSHOT-jar-with-dependencies.jar
java -jar target/zkui-2.0-SNAPSHOT-jar-with-dependencies.jar
'''
        }

      }
    }

  }
}