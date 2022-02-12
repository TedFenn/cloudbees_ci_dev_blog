@Library('common_shared_blog_lib') _

pipeline {
    agent {
        kubernetes{
            yaml libraryResource('maven-pod.yaml')
        }
    }
    stages {
        stage ("cleverness") {
            steps {
                script {
                    echo "I'm running a custom pipeline!"
                }
            }
        }
    }
}