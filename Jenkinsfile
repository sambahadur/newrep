pipeline {
    agent any

    stages {
        stage('Build') {
            steps {
                sh 'python3 -m py_compile code2.py'
            }
        }
	stage('install pytest'){
	 steps{
	    sh'pip3 install pytest'}
        stage('Test') {
            steps {
                sh 'python3 -m pytest'
            }
        }
        }
    
}
