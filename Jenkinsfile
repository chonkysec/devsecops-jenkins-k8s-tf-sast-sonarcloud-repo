pipeline {
  agent any
  tools { 
        maven 'Maven_3_5_2'  
    }
   stages{
    stage('CompileandRunSonarAnalysis') {
            steps {	
		sh 'mvn clean verify sonar:sonar -Dsonar.projectKey=asgbuggywebapp6 -Dsonar.organization=asgbuggywebapp6 -Dsonar.host.url=https://sonarcloud.io -Dsonar.token=824d99c44e21ce59e1b679763da90554f9730039'
			}
        } 
  }
}
