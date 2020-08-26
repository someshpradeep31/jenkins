pipeline {
         agent any
         stages {
                 stage('One') {
                 steps {
                     echo 'Hi,I am Somesh Pradeep'
                 }
                 }
                 stage('Two') {
                 steps {
                    input('Do you want to proceed?')
                 }
                 }
                 stage('Three') {
                 when {
                       not {
                            branch "master"
                       }
                 }
                 steps {
                       echo "Hello"
                 }
                 }
                 
                 
                            stage('Four') {
                           steps {
                                echo "Testing the scripts"
                           }
                           }
                            stage('Five') {
                              
                              steps {
                                echo "Deploying the project"
                              }
                           }
                           
                           
              }
}
