pipeline {
    agent any
    
    stages {
        stage('Example Build') {
            steps {
                sh 'pwd'
		sh 'cd $pwd'
		echo 'there are sh 'ls | wc -l'' 
		echo 'count the number of files please!'
            }
        }
        stage('Example Test') {
           
            steps {
                echo 'Hello, JDK'
                sh 'java -version'
            }
        }
    }

  post {
	always {
		echo 'This Jenkinsfile pipeline training was susccefully completed!'
	}
	  failure {
	  	echo 'The runtime failed this time please!'
	  }
 }
}
	
