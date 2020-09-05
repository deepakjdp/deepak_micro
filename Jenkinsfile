node {
  stage('SCM') {
    git 'https://github.com/deepakjdp/deepak_micro.git'
  }
  stage('SonarQube analysis') {
    def scannerHome = tool 'sonar_scan';
    
    withSonarQubeEnv('sonarqube') { // If you have configured more than one global server connection, you can specify its name
      def scannerHome1 = bat "cd ${scannerHome}/bin"
        echo $scannerHome1
        bat 'C:\Program Files (x86)\Jenkins\tools\hudson.plugins.sonar.SonarRunnerInstallation\sonar_scan\bin\sonar-scanner'
        
    }
  }
}
