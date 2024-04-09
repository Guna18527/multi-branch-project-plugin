pipeline {
    agent any
	
    tools {
        maven 'maven3'
    }    
    stages {
        stage ('git checkout') {
            steps {
                git ' https://github.com/Guna18527/multi-branch-project-plugin.git'
            }
        }
	 stage('maven') {
            steps {
                sh 'mvn clean compile'
            }
        }
	    
        stage('echo'){
		steps{
		    echo 'Echo steps running'
	    }
	}	
	stage('Test') {
            steps {
                echo 'test'
            }
        }
    }
}
