pipeline {
   
   agent any
   
     
   stages {
        stage('Build') { 
            
                echo 'Maven Build in Progress..'
				try{
				sh 'mvn clean package'
				}catch(Exception e) {
				//Not Found 
				}				
            
        }
		stage('Test') {
            steps {
                echo 'Testing..'
            }
        }
        stage('Deploy') {
            steps {
                echo 'Deploying....'
            }
        }
  }
}