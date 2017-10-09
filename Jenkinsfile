node {

   stage 'checkout from GitHub'
        echo 'Checking out files'
	checkout scm
	

   stage 'Build using maven'
         echo 'running clean install using maven'
	 sh "${tool 'Maven Latest'} -B verify"
	 sh "${tool 'Maven Latest'} clean install"
     

     }
