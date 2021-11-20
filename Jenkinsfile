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
    }
}