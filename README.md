# jenkins_ssh


pipeline{
        agent any
        stages{
            stage('Create file'){
                steps{
                        sshagent(['cb38f8ec-2d0a-4696-bd26-8e23756d0756']) {
                                sh '''
                                ssh ubuntu@18.134.12.28
                                touch prova.txt 
                                '''
                                     }                         
                }
            }
        }
}
