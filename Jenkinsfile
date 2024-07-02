pipeline {
    agent any
    stages {
        stage('build') {
            steps {
                sh 'python --version'
		sh 'pwd'
		sh '''
		    cd /Users/fanzexin/jenkins_test
		    ls
		'''
            }
        }
	stage('build check') {
            steps {
                input "Does the build look ok?"
            }
        }
    }
    post {
    	success {
             echo 'build success'
    	}
  }
}
