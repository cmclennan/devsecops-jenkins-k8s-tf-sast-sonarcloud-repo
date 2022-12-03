pipeline {
  agent any
  tools { 
        maven 'Maven_3.5.2'  
    }
   stages{
    stage('CompileandRunSonarAnalysis') {
            steps {	
		sh 'mvn clean verify sonar:sonar -Dsonar.projectKey=camtestbuggywebapp -Dsonar.organization=camtestbuggywebapp -Dsonar.host.url=https://sonarcloud.io -Dsonar.login=6441affdf0663c222bae153e5afaea4ac8d737a8'
			}
        } 
  }
}
