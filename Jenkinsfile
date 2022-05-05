node {
  stage('SCM') {
    checkout scm
  }
  stage('SonarQube Analysis') {
    dir('./TransactionService') {
      sh "./gradlew sonarqube"
    }
  }
}