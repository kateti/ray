pipeline {
    agent any
    
    stages {
        stage('Example Build') {
            steps {
                sh 'pwd'
		sh 'cd $pwd'
		sh 'ls | wc -l'
		echo 'that is counted number of files please!'
            }
		post {
			success {
			   echo 'This pipeline tage ran without error!'
			}	
			failure {
				echo 'You need to review your code please!'
			}
		}
        }
        stage('Example Test') {
           
            steps {
                echo 'Hello, JDK'
                sh 'java -version'
            }
        }
    }
