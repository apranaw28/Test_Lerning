pipeline {
        agent any 
		
	   stages {
        stage('Init') {
            steps {
               echo 'This is an Initialization phase.'
            }
        } 
		}
        stage('Build') {
            steps {
                echo 'Build Phase....'
                sh '/opt/maven/bin/mvn clean install'	
            }
        }
        stage('Unit Test') {
            steps {
               echo 'Skipping Unit Tests for now....'
            }            
        }
		
		}