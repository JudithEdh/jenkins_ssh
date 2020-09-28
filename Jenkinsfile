pipeline{
        agent any
        stages{
            stage('Create file'){
                steps{
                        sshagent(['ubuntu']) {
                             
                                sh 'ssh -o StrictHostKeyChecking=no ubuntu@18.134.12.28 uptime'
                                sh '''
                                ssh -v ubuntu@18.134.12.28<<-'ENDSSH'
                                #!/bin/bash
                                pwd
                                touch yes.txt
                                ENDSSH
                                '''
                                     }                         
                }
            }
        }
}
