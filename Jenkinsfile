pipeline {
  agent any
  stages {
    stage('Build') {
      steps {
        tool(name: 'maven 3.6.3', type: 'mvn')
        sh 'mvn -Dmaven.test.skip=true clean install'
        echo 'Building Pipeline'
      }
    }

  }
}