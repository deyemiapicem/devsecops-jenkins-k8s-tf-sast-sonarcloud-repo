pipeline {
  agent any
  tools { 
        maven 'Maven_3_5_2'  
    }
   stages{
    stage('CompileandRunSonarAnalysis') {
            steps {	
		sh 'mvn clean verify sonar:sonar -Dsonar.projectKey=asgbuggywebapplicatio -Dsonar.organization=asgbuggywebapplicatio -Dsonar.host.url=https://sonarcloud.io -Dsonar.token=b3b68b64382edc099d297ec63d4c3242f8535232'
			}
        } 
  }
}
