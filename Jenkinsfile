pipeline {
    agent any

    stages {
        stage('Update browser') {
            steps {
                nodejs(nodeJSInstallationName: 'sample') {
                    sh 'npm i caniuse-lite browserslist'
                }
            }
        }
        stage('Install') {
            steps {
                nodejs(nodeJSInstallationName: 'sample') {
                    sh 'npm install'
                }
            }
        }
        stage('Build') {
            steps {
                nodejs(nodeJSInstallationName: 'sample') {
                    sh 'npm run build'
                }
            }
        }
    }
}
