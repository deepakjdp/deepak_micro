pipeline {
        agent none
        stages {
          stage("build & SonarQube analysis") {
            agent any;
            def scannerHome = tool 'SonarScanner 4.0';  
            steps {
              withSonarQubeEnv('sonarqube') {
                      sh "${scannerHome}/bin/sonar-scanner"
              }
            }
          }
          stage("Quality Gate") {
            steps {
              timeout(time: 1, unit: 'HOURS') {
                waitForQualityGate abortPipeline: true
              }
            }
          }
        }
      }
