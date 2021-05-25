pipeline {
  agent any 
  
    stages {
	
	   stage ('compile') {
	
	      steps {
	      withMaven(maven : 'maven version') {
		  sh 'mvn clean compile'
		      }
		    }
		  }
		  
		  
		  stage ('test') {
	
	      steps {
	      withMaven(maven : 'maven version') {
		  sh 'mvn clean test'
		      }
		    }
		  }
		  
		  
		  stage ('deplyment') {
	
	      steps {
	      withMaven(maven : 'maven version') {
		  sh 'mvn clean deploy'
		  
		      }
		    }
		  }
        }

    }
