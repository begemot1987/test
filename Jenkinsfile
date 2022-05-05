node {
  stage('SCM') {
    checkout scm
  }
  stage('SonarQube Analysis') {
    sh "./gradlew sonarqube"
  }
}