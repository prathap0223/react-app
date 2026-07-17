pipeline{
    agent any
    stages{
        stage('Build') {
            steps {
                sh 'sudo docker build -t react-external .'
            }
        }
        stage('Run') {
            steps {
                sh 'sudo docker run -d -p 3000:3000 react-external'
            }
        }
    }
}