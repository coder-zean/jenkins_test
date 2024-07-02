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
        	mail to: 'fanzexin@insta360.com',
             	subject: "Failed Pipeline: ${currentBuild.fullDisplayName}",
             	body: "Something is wrong with ${env.BUILD_URL}"
    	}
  }
}
