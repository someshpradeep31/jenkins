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
                 parallel { 
                            stage('Testing') {
                           steps {
                                echo "Testing the script"
                           }
                           }
                            stage('Deploying') {
                              
                              steps {
                                echo "Deploying the project"
                              }
                           }
                           }
                           }
              }
}
