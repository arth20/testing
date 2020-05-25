pipeline {
	environment {
    dockerImage = ''
  }
  agent any
    
  tools {nodejs "localnode"}
    
  stages {
        
    stage('Git') {
      steps {
        git 'https://github.com/arth20/youtube'
      }
    }
     
    stage('Install dependencies') {
		steps{
             		sh 'npm install'
		}
	}
		stage('Test') {				
			  steps{
				
					
                        sh 'npm test'
			
			}
			  
			
	}
     	
	  
  }
}
