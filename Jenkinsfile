pipeline {
    //agent any
    agent {
       node {
          label 'workstation'
       }
     }
     environment{
     Test_URL = "google.com"
     SSH=credentials("centos-ssh")
     }

    stages {

        stage('Stage 1- Code') {
            steps {
                echo 'Hello World Stage-1'
                echo Test_URL
                echo SSH
                sh 'env'

            }
        }

        stage('Stage 2- Test') {
            steps {
                echo 'Hello World Stage-2'
            }
        }

        stage('Stage 3- Code Quality') {
            steps {
                echo 'Hello World Stage-3'
            }
        }

        stage('Stage 4- Code Security') {
            steps {
                echo 'Hello World Stage-4'
            }
        }
    }
}