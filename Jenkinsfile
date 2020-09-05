node {
  stage('SCM') {
    git 'https://github.com/deepakjdp/deepak_micro.git'
  }
  stage('SonarQube analysis') {
    def scannerHome = tool 'sonar_scan';
    withSonarQubeEnv('sonarqube') { // If you have configured more than one global server connection, you can specify its name
      sh "${scannerHome}/bin/sonar-scanner"
    }
  }
}
