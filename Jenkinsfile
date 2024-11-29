pipeline {
    agent any

    stages {
        
        stage('Build with Maven'){
	     steps{
	     	 echo "MAVEN"
		 sh 'mvn package'
	      }
        }
        stage('Build docker'){
	     steps{
		 echo "DOCKERIZE"
		 sh "pwd"
		 sh "ls"
		 sh 'docker build -t khouloudbenali/devops:1.0 .'
	      }
        }
    }
}
