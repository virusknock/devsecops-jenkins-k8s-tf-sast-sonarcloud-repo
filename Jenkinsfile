pipeline {
  agent any
  tools { 
        maven 'maven_3_2_5'  
    }
   stages{
    stage('CompileandRunSonarAnalysis') {
            steps {	
		sh 'mvn clean verify sonar:sonar -Dsonar.projectKey=virusknock -Dsonar.organization=virusknock -Dsonar.host.url=https://sonarcloud.io -Dsonar.token=86bb206426fbc5881560884a2b8758f4266f4b17'
			}
        } 
  }
}
