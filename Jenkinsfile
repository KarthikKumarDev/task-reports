pipeline {
     agent any
     stages {
        stage("Build") {
            steps {
                 nodejs(nodeJSInstallationName: 'Node 6.x', configId: '<config-file-provider-id>') {
                    sh "sudo yum npm install"
                sh "sudo yum npm run build"
                }   
            }
        }
    }
}
