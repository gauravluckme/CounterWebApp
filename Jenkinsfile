pipeline {
   
   agent any
   
     
   stages {
        stage('Build') { 
            steps {
                echo 'Maven Build in Progress..'
		sh 'mvn clean package -DskipTests'
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
