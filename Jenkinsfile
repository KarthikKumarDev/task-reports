pipeline {
     agent any
     stages {
        stage("Build") {
            steps {
                sh "sudo yum apt-get install npm"
                sh "sudo yum npm install"
                sh "sudo yum npm run build"
            }
        }
    }
}
