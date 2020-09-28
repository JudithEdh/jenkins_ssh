pipeline{
        agent any
        stages{
            stage('Create file'){
                steps{
                        sshagent(['ubuntu']) {
                                sh '''
                                ssh ubuntu@18.134.12.28
                                pwd
                                touch prova.txt 
                                '''
                                     }                         
                }
            }
        }
}
