pipeline {
  agent any
  tools { 
        maven 'Maven_3_5_2'  
    }
   stages{
    stage('CompileandRunSonarAnalysis') {
            steps {	
		sh 'mvn clean verify sonar:sonar -Dsonar.projectKey=devsecopstone -Dsonar.organization=devsecopstone -Dsonar.host.url=https://sonarcloud.io -Dsonar.login=e899057f2c762ff7033aca139dc641b08e483894'
			}
        } 
  }
}
