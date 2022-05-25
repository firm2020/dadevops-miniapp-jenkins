pipeline {
    agent {
        docker {
            image 'maven:3-openjdk-11'
            args '-v $HOME/.m2:/root/.m2 -u root'
        }
    }
    stages {
        stage('Build') {
            steps {
                sh 'mvn --version'
            }
        }
    }
}
