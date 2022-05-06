node {
    stage('SCM') {
        checkout scm
      }
      stage('SonarQube Analysis') {
        sh "java -version"
        dir('./demo') {
          sh "./gradlew sonarqube"
        }
      }
}