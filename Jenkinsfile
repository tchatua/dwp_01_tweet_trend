pipeline {
    agent {
        node {
            label 'maven-labels'
        }
    }
environment {
    PATH = "/opt/apache-maven-3.9.6/bin:$PATH"
}
    stages {
        // stage('Clone GitHub Repository') {
        //     steps {
        //         git branch: 'main', url: 'https://github.com/tchatua/dwp_01_tweet_trend.git'
        //     }
        // }
        stage ('Build on Maven (Jenkins Worker Node)') {
            steps {
                sh 'mvn clean deploy'
            }
        }
    }
}
