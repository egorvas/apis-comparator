pipeline {
     agent { label "builder" }
     options {
        disableConcurrentBuilds()
     }
     stages {
        stage('Run script') {
            steps {
                script{
                        sh 'npm i'
                        sh 'logs/getTokenInfo.sh'
                }
            }
        }
    }
}