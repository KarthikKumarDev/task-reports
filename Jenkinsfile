pipeline {
     agent any
     stages {
        stage("Build") {
            steps {
                sh "yum npm install"
                sh "yum npm run build"
            }
        }
    }
}
