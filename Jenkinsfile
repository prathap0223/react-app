pipeline{
    agent any
    triggers{
        cron("h/2"****)
    }
    stages{
        stage('Build')
        {
            steps{
                sh "sudo docker build -t myapp ."
            }
        }
        stage('run')
        {
            steps{
                sh "sudo docker run -d --name react-app-test -p 3000:3000 myapp"
            }
        }
    }
}