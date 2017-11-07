pipeline {
   
   agent any
   
     
   stages {
        stage('Build') { 
            steps {
                echo 'Maven Build in Progress..'
				try{
				sh 'mvn clean package'
				}catch{Exception e) {
				//Not Found 
				}				
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