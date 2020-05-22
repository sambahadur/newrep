pipeline {
    agent any

    stages {
        stage('build') {
            steps {
                sh 'python3 -m py_compile src.py'
            }
        }
	stage('install pytest'){
	 steps{
	    sh'pip3 install pytest --user'}
	    }
        stage('test') {
            steps {
                sh 'python3 -m pytest --user'
            }
        }
    }
}
