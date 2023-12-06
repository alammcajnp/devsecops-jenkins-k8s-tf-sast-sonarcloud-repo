pipeline {
  agent any
  tools { 
        maven 'Maven_3_5_2'  
    }
   stages{
    stage('CompileandRunSonarAnalysis') {
            steps {	
		sh 'mvn clean verify sonar:sonar -Dsonar.projectKey=alamjnp12 -Dsonar.organization=alamjnp12 -Dsonar.host.url=https://sonarcloud.io -Dsonar.login=0cf8cd7a0453d4105a79736afed033a5e7057ce2'
			}
        } 
  }
}
