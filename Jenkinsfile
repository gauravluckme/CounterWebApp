.shpipeline {
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
      		        sh 'cp C:/Users/gaurav.pant/Downloads/onlinequiz/CounterWebApp.war C:/Users/gaurav.pant/Downloads/apache-tomcat-7.0.82/apache-tomcat-7.0.82/webapps/'
    		        sh 'cd C:/Users/gaurav.pant/Downloads/apache-tomcat-7.0.82/apache-tomcat-7.0.82/bin'
			sh 'startup.sh'
    }
	 }

  	   }
}
