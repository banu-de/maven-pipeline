pipeline {
  agent any 
  
    stages {
	
	   stage ('compile') {
	
	      step {
	      withMaven(maven : 'maven version') {
		  sh 'mvn clean compile'
		      }
		    }
		  }
		  
		  
		  stage ('test') {
	
	      step {
	      withMaven(maven : 'maven version') {
		  sh 'mvn clean test'
		      }
		    }
		  }
		  
		  
		  stage ('deplyment') {
	
	      step {
	      withMaven(maven : 'maven version') {
		  sh 'mvn clean deploy'
		  
		      }
		    }
		  }
        }

    }
