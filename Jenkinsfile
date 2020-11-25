pipeline {
        agent any 
		
	    stage('checkout')
		{
		step{echo 'checkout'}
		}
		stage ('build_condition')
		{
		step{input ('Do you want to proceed')}
		}
		stage ('build')
		{
		
		steps{echo 'Building the application'}
		}
		
		}