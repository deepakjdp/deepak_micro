node {
  stage('SCM') {
    git 'https://github.com/deepakjdp/deepak_micro.git'
  }
  stage('SonarQube analysis') {
    def scannerHome = tool 'sonar_scan';
    def scannerHome = tool 'sonar_scan';
    def scannerHome = tool 'sonar_scan';
    def scannerHome = tool 'sonar_scan';
    def test = tool for merge test;  
    def scannerHome = tool 'sonar_scan';
    def scannerHome = tool 'sonar_scan';
    echo "etst"
    echo "testing"
    withSonarQubeEnv('sonarqube') { // If you have configured more than one global server connection, you can specify its name
      def scannerHome1 = bat "cd ${scannerHome}/bin"
        echo "test"
        // echo $scannerHome1
        //bat 'C:\Program Files (x86)\Jenkins\tools\hudson.plugins.sonar.SonarRunnerInstallation\sonar_scan\bin\sonar-scanner'
        bat """
        cd C:\\Program Files (x86)\\Jenkins\\tools\\hudson.plugins.sonar.SonarRunnerInstallation\\sonar_scan\\bin
        sonar-scanner -Dsonar.projectKey=deepak_micro -Dsonar.java.binaries="C:\\Program Files (x86)\\Jenkins\\workspace\\pipeline_one\\src\\main\\java" -Dsonar.projectVersion=1.0 -Dsonar.projectBaseDir="C:\\Program Files (x86)\\Jenkins\\workspace\\pipeline_one\\src\\main\\java" -Dsonar.sources="C:\\Program Files (x86)\\Jenkins\\workspace\\pipeline_one\\src\\main\\java"     
         """ 
    }
  }
}
