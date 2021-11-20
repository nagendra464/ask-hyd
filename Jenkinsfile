// Declarlative pipeline
pipeline{
    agent { node { label 'Docker'} }
    stages {
        stage ('clone the code'){
            steps {
                sh 'git clone https://github.com/nagendra464/ask-hyd.git'
            }
        }
        stage ('maven'){
            steps {
                sh 'mvn clean install'
            }
        }
        stage ('build docker image'){
            steps { 
                sh 'docker build -t nagendra464/tom-deploy:latest .'
            }
        }
    }
}