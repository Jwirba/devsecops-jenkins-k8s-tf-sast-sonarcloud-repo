pipeline {
  agent any
  tools { 
        maven 'Maven_3_5_2'  
    }
   stages{
    stage('CompileandRunSonarAnalysis') {
            steps {	
		sh 'mvn clean verify sonar:sonar -Dsonar.projectKey=jde1 -Dsonar.organization=jde1 -Dsonar.host.url=https://sonarcloud.io -Dsonar.login=b7517cc49bdddca0c1cf6d55c2f1107a66bd1092'
			}
        } 
  }
}
