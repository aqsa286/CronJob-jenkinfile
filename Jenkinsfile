pipeline {
    agent any

    stages {
        stage('Execute') {
            steps {
                git branch: 'main', credentialsId: 'cron_credential', url: 'https://github.com/aqsa286/trail_repo.git'
                script{
                sh '''
                 ls -ltr
                 ./trail.sh
                '''
                }
            }
        }
    }
}
