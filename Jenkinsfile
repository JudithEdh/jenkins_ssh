pipeline{
        agent any
        stages{
            stage('Create file'){
                steps{
                  sh '''
                  #! /bin/bash
                  ssh try@18.134.12.28
                  touch prova.txt       
                  '''
                }
            }   
         }
}
