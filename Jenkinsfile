pipeline{
    agent any
    stages{
        stage('Clone'){
            steps{
                git 'https://github.com/quoc2721/admin_dashboard.git'
            }
        }
    }
    post {
        always {
           mail bcc: '', body: 'Thông báo vừa có 1 push build project update', cc: 'admindashboard.vn, quoc020721@gmail.com', from: '', replyTo: '', subject: 'Jenkins Notification ', to: 'quoc020721@gmail.com'
        }
    }
}