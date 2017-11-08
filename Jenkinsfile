pipeline {
   agent any    
   stages {
        stage('Build') { 
            steps {
                echo 'Maven Build in Progress..'
		sh 'mvn -B -DskipTests clean package' 
			}
		  }
	 stage('Deploy') {
		 steps {
      			echo 'Maven Deployment in Progress..'
			sh 'mvn tomcat7:deploy'
		    }
	 }

  	   }
}
