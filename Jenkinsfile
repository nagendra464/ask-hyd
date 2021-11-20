// Declarlative pipeline
pipeline{
    agent { node { label 'Docker'} }
    stages {
        stage ('clone the code'){
            steps {
                sh 'https://github.com/nagendra464/ask-hyd.git'
            }
        }
    }
}