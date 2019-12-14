pipeline {
    agent {
        node {
            label 'terminator'
        }
    }
    environment {
        CC_NAME = 'Build Machine for Human'
        PROJECT_NAME='DECLARATIVE PIPELINE'
    }
    stages {
        stage('Dummy Stage') {
            steps {
                script {
                    if (isUnix()) {
                        sh "echo '$CC_NAME'"
                    
                    } else {
                        bat "echo '$CC_NAME'"
                    }
                }

            }
            post {
                always {
                    sh "echo Hello World"
                }
            }
        }
        stage('Another Dummy'){
            steps{
                sh 'echo Another dummy'
                sh "echo '$PROJECT_NAME'"
            }
        }
    }
    post {
        always {
            sh "echo  Hell from Jenkin"
        }
    }

}