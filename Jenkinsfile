pipeline {
  agent any
  stages {
    stage('Build') {
      steps {
        tool(name: 'maven 3.6.3', type: 'maven')
        sh 'withEnv( ["PATH+MAVEN=${tool maven 3.6.3}/bin"] )'
        sh 'mvn -Dmaven.test.skip=true clean install'
        echo 'Building Pipeline'
      }
    }

  }
}