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
    }
    post {
    	success {
             echo 'build success'
    	}
  }
}
