node {
  stage('SCM') {
    checkout scm
  }
  stage('SonarQube Analysis') {
    steps {
      dir('./TransactionService') {
          sh "./gradlew sonarqube"
        }
    }
  }
}