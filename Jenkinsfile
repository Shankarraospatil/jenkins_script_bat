pipeline {
    agent any

    stages {

        stage('Clone Repository') {
            steps {
                git branch: 'main',
                    url: 'https://github.com/Shankarraospatil/jenkins_script_bat.git'
            }
        }

        stage('Build') {
            steps {
                bat 'build.bat'
            }
        }

        stage('Test') {
            steps {
                bat 'test.bat'
            }
        }

        stage('Deploy') {
            steps {
                bat 'deploy.bat'
            }
        }

        stage('Create File') {
            steps {
                bat 'createfile.bat'
            }
        }
    }
}
