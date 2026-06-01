@Library('Library_function') _

pipeline {
    agent any

    stages {

        stage('Load Config') {
            steps {
                script {
                    cfg = load 'deploy-config.groovy'
                }
            }
        }

        stage('Deploy') {
            steps {
                script {
                    opensearchDeploy(cfg)
                }
            }
        }
    }
}