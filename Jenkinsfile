pipeline {
  agent any
  tools { 
        maven 'Maven_3_5_2'  
    }
   stages{
    stage('CompileandRunSonarAnalysis') {
            steps {	
		sh 'mvn clean verify sonar:sonar -Dsonar.projectKey=buggyapp2024 -Dsonar.organization=buggyapp2024 -Dsonar.host.url=https://sonarcloud.io -Dsonar.token=deb7eebafc9c18397e13cabb009f71245dc5ed36'
			}
        } 
  }
}
