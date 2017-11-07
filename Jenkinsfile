pipeline {
   
   agent any
   
     
   stages {
        stage('Build') { 
            steps {
                echo 'Maven Build in Progress..'
		    withMaven(maven : 'maven_3_5_2'){
				sh 'mvn clean package -DskipTests'
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
