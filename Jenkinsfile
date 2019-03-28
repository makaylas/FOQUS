pipeline {
    agent { docker { image 'python:3.5.1' } }
    stages {
        stage('build') {
            steps {
                sh 'root:sudo pip install --upgrade pip'
                sh 'root:sudo pip install -r requirements.txt'
                sh 'python setup.py install'
            }
        }
    }
}
