node {
  stage('SCM') {
    checkout scm
  }
  stage('SonarQube Analysis') {
    dir('../demo') {
      sh "./gradlew sonarqube"
    }
  }
}