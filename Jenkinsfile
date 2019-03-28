pipeline {
    agent { docker { image 'python:3.5.1' } }
    stages {
        stage('build') {
            script {
                pip install -r requirements.txt
                python setup.py install
            }
        }
    }
}
