pipeline {
	
    agent {label 'docker_sanjay'}
    stages {
	      stage ('DEV') {
            steps {
                  sh 'echo "Hi Sanjay its DEV STAGE"'
                }
            }  
        stage('UAT') {
            steps {
		              sh 'echo "Hi Sanjay its UAT STAGE"'
            }
        }
	      stage('Approval Step'){
            steps{
                  sh 'echo "Hi Sanjay its PROD STAGE"'
        }
     }
  }
    post {
    success {
        sh 'echo "Pipeline Works"'
    }
    failure {
        script {
            sh 'echo "Pipeline Failed"'
        }
    }
    }
}
