pipeline{
	       agent any
	       
	       stages{
	       
	              stage('compile stage'){
	                      steps{
	                             withMaven(maven : 'mvn'){
	                                    sh 'mvn clean compile'
	                             }
	                      }
	              }
	              
	              stage('Testing stage'){
	                      steps{
	                             withMaven(maven : 'mvn'){
	                                    sh 'mvn test'
	                             }
	                      }
	              }
	              
	       }
	}
