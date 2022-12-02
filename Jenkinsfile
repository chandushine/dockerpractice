pipeline {
    agent { label 'docker' }
    stages {
        stage (clone) {
            steps{
                git url: "https://github.com/chandushine/dockerpractice.git",
                branch: "master"
            }
        }
        stage (build) {
            steps {
                sh 'docker image build -t chandu:1.0'
            }
        }
    }
}