pipeline {
  agent any 
  
    stages {
	
	   stage ('compile') {
	
	      steps {
	      withMaven(maven : 'maven 3.8.1') {
		  sh 'mvn clean compile'
		      }
		    }
		  }
		  
		  
		  stage ('test') {
	
	      steps {
	      withMaven(maven : 'maven 3.8.1') {
		  sh 'mvn clean test'
		      }
		    }
		  }
		  
		  
		  stage ('deplyment') {
	
	      steps {
	      withMaven(maven : 'maven 3.8.1') {
		  sh 'mvn clean deploy'
		  
		      }
		    }
		  }
        }

    }
