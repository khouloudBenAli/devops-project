pipeline {
    agent any

    stages {
       
        stage('Clone Master Branch'){
	     steps{
		 git url: 'https://github.com/khouloudBenAli/devops.git'
	      }
        }
        
        stage('Build with Maven'){
	     steps{
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
