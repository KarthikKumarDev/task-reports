pipeline {
    agent any

    stages {
        stage('Update browser') {
            steps {
                nodejs(nodeJSInstallationName: 'sample') {
                    sudo 'npx browserslist@latest --update-db'
                }
            }
        }
        stage('Install') {
            steps {
                nodejs(nodeJSInstallationName: 'sample') {
                    sudo 'npm install'
                }
            }
        }
        stage('Build') {
            steps {
                nodejs(nodeJSInstallationName: 'sample') {
                    sudo 'npm run build'
                }
            }
        }
    }
}
