@Library('opensearch-library') _

def cfg = load 'deploy-config.groovy'

pipeline {
    agent any

    stages {
        stage('Deploy') {
            steps {
                script {
                    opensearchDeploy(cfg)
                }
            }
        }
    }
}