pipeline {
 agent any
  stages {
      stage('Pull') {
         steps {
             git 'https://github.com/channagouda0909/ctsdec1batch.git'
         }
      }
      stage('Package') {
         steps {
            bat 'mvn package'
         }
      }
      stage('Execute') {
         steps {
            bat 'java -jar "C:/ProgramData/Jenkins/.jenkins/workspace/job55/target/cts-1.0-SNAPSHOT.jar"'
         }
      }
   }
}
