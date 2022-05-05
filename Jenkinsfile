node {
  stage('SCM') {
    checkout scm
  }
  stage('SonarQube Analysis') {
    dir('./demo2') {
      sh "./gradlew sonarqube"
    }
  }
}