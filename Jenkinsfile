pipeline {
  agent any
  tools { 
        maven 'Maven_3_5_2'  
    }
   stages{
    stage('CompileandRunSonarAnalysis') {
            steps {	
		sh 'mvn clean verify sonar:sonar -Dsonar.projectKey=camtestbuggywebapp -Dsonar.organization=camtestbuggywebapp -Dsonar.host.url=https://sonarcloud.io -Dsonar.login=963a4237d0fa6cc3273e00510df0eb004673323e'
			}
        } 
  }
}
