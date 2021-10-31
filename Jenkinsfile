pipeline {
	agent any
	tools {
    	maven 'maven-new'
	}
	stages {
    	stage("Checkout") {   
        	steps {               	 
            	git url: 'https://github.com/melvincv/jenkins-spring-boot-build.git'          	 
           	 
        	} 
    	}
    	stage('Build') {
        	steps {
				sh "mvn compile"  	 
        	}
    	}
   	 
    	stage("Unit test") {          	 
        	steps {
				sh "mvn test"          	 
			}
	    }	
	}
}