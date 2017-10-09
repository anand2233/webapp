node {
   def mvnHome
      stage 'checkout from GitHub'
            // Get some code from a GitHub repository
	          //git 'https://github.com/pratikjais123/webapp.git'
		        // Get the Maven tool.
			      // ** NOTE: This 'M3' Maven tool must be configured
			            // **       in the global configuration.           
				          mvnHome = tool 'Maven'
	stage 'Build using maven'
	       // Run the maven build
	           if (isUnix()) {
	              sh "'${mvnHome}/bin/mvn' -Dmaven.test.failure.ignore clean package"
			    } else {
			      bat(/"${mvnHome}\bin\mvn" -Dmaven.test.failure.ignore clean package/)								     }
				}							        
												}
