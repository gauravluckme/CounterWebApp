pipeline {
   agent any    
   stages {
        stage('Build') { 
            steps {
                echo 'Maven Build in Progress..'
		sh 'mvn -B -DskipTests clean package' 
			}
		  }
  	   }
}
