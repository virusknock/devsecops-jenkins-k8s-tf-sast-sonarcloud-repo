pipeline {
  agent any
  tools { 
        maven 'maven_3_2_5'  
    }
   stages{
    stage('CompileandRunSonarAnalysis') {
            steps {	
		sh 'mvn clean verify sonar:sonar -Dsonar.projectKey=virusknock -Dsonar.organization=virusknock -Dsonar.host.url=https://sonarcloud.io -Dsonar.token=fd3cfb35e4c9c59edfab315e289190e318d745a0'
			}
        } 
  }
}
