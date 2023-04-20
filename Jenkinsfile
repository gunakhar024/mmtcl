pipeline {
   agent any
   stages {
       stage('Build Code') {
           steps {
               sh """
               echo "Building Artifact for project samplewebapp"
			   """
               
           }
       }
       stage('Reading branch wise')
       {
       when
       {
       branch "prod*"
       }
       steps
       {
       echo " It is only for prod branch"
       }
       }

       stage('Deploy Code') {
	   
          steps {
               sh """
               echo "Deploying Code"
			   """
               
          }
      }
      }
      }
