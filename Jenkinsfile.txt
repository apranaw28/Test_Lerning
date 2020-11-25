pipeline {
        agent any 
	    stage{'one'}
		{
		step{echo 'Hello from the other side'}
		}
		stage ('two')
		{
		step{input ('Do you want to proceed?')}
		}
		stage ('three')
		{
		when{not {branch "master"}}
		}
		steps{echo "Hello"}
        }
 