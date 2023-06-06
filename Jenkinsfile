pipeline {
    agent any
    
    stages {
        stage('Example Build') {
            steps {
                sh 'pwd'
		sh 'cd $pwd'
		sh 'ls | wc -l'
		ech 'count the number of files please!'
            }
		post {
			success {
			   echo 'This pipeline tage ran without error!'
			}	
			unsuccessful {
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

  }
	
