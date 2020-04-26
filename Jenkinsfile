pipeline {
  agent any
  stages {
    stage('Stage1') {
      parallel {
        stage('Stage1') {
          steps {
            sh 'echo Hello'
            sh 'echo "Hi"'
          }
        }

        stage('Staging1b') 
		node {
        	checkout scm
			sh 'echo "checkout scm successfully"'
          }
        }
      }
    }
}
