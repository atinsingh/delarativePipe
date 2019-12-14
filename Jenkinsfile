pipeline {
        agent {
                node{
                       label 'terminator'
                }
        }
        environment{
            CC_NAME='Build Machine for Human'
        }
        stages{
            stage('Dummy Stage'){
                steps{
                   // if(isUnix()){
                        sh "echo '$CC_NAME'"
                  //  }else {
                    //    bat "echo '$CC_NAME'"
                    //}
                    
                }
                post{
                    always{
                        sh "echo Hello World"
                    }
                }
            }
        }
        post {
            always{
                sh "echo  Hell from Jenkin"
            }
        }
        
}
