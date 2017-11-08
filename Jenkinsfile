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
      		        sh 'cp C:\Program Files (x86)\Jenkins\workspace\Pipeline@2\target\CounterWebApp.war C:/Users/gaurav.pant/Downloads/apache-tomcat-7.0.82/apache-tomcat-7.0.82/webapps/CounterWebApp.war'
    		        sh 'cd C:\Users\gaurav.pant\Downloads\apache-tomcat-7.0.82\apache-tomcat-7.0.82\bin'
			sh 'startup'
    }
	 }

  	   }
}
