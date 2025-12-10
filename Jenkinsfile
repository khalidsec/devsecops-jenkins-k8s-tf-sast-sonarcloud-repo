pipeline {
  agent any
  tools { 
        maven 'Maven_3_5_2'  
    }
   stages{
    stage('CompileandRunSonarAnalysis') {
            steps {	
		sh 'mvn clean verify sonar:sonar -Dsonar.projectKey=khalidbuggywebapp -Dsonar.organization=khalidbuggywebapp -Dsonar.host.url=https://sonarcloud.io -Dsonar.token=23903c705127c9c03f8ed15aa126f5a6a0bc400d'
			}
        } 
  }
}
