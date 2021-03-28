pipeline {
  agent any
  tools { 
    maven 'maven 3.6.3' 
  }	
  stages {
    stage ("Build") {
      steps {
	    sh "mvn -Dmaven.test.skip=true clean install" 
	    echo 'Building..'
      }  
    } 
  }
} 
