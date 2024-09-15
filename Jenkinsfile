pipeline {
  agent any
  tools { 
        maven 'maven_3_2_5'  
    }
   stages{
    stage('CompileandRunSonarAnalysis') {
            steps {	
		sh 'mvn clean verify sonar:sonar -Dsonar.projectKey=virusknock -Dsonar.organization=virusknock -Dsonar.host.url=https://sonarcloud.io -Dsonar.token=be2c401528cf9333a0da1df354853940d748442b'
			}
        } 
  }
}
