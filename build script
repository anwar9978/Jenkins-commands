pipeline {
    agent any
    environment {
        PATH = "/opt/maven/bin:$PATH"
    }
    stages {
        stage('git clone') {
            steps {
                git url: 'https://github.com/anwar9978/IRCTC.git', branch:'main'
            }
        }
        stage('build2') {
            steps {
                sh 'mvn clean install'
            }
        }
        stage('deploy') {
            steps {
                echo "deploying"
            }
        }
    }
}
