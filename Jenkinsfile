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
            mail bcc: '', body: 'Thông báo kết quả build', cc: 'admindashboard.vn, quoc020721@gmail.com', from: '', replyTo: '', subject: 'Notification', to: 'quoc020721@gmail.com'
        }
    }
}