pipeline {
    agent { docker { image 'python:3.5.1' } }
    stages {
        stage('build') {
            steps {
                pip install -r requirements.txt
                python setup.py install
            }
        }
    }
}
