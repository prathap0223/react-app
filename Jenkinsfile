pipeline{
    agent any
    stages{
        stage('Build') {
            steps {
                sh 'docker build -t react-external .'
            }
        }
        stage('Run') {
            steps {
                sh 'docker run -d -p 3000:3000 react-external'
            }
        }
    }
}