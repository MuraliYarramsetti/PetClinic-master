pipeline{
    agent any
	
	stages {
	   stage ('Compile stage'){
	     steps {
		 
	      withMaven(maven : 'Maven350') {
		  sh 'mvn clean compile'
				}
			}
		  }
		stage ('Testing Stage')
		  steps {
		withMaven(maven : 'Maven350') {
		  sh 'mvn test'		 }
		}
	}
	}
