//SCRIPTED

//DECLARATIVE
pipeline {
	//agent any 
	agent { docker { image 'maven:3.9.9'} }
	stages {
		stage('Build') {
	        steps {
				sh 'mvn --version'
				echo "Build"
			}   
		}
		stage('Test') {
	        steps {
				echo "Test"
			}
		}
		stage('Intergration Test') {
	        steps {
				echo "Intergration Test"
			}
		}
	} 
	
	post {
		always {
			echo 'Im awesome. I run always'
		}
	    success {
		    echo 'I run when you are successful'
	    }
		failure {
		    echo 'I run when you fail'
	    }
	}
}
	

