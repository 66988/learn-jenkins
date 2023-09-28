pipeline {
    //agent any
    agent {
       node {
          label 'workstation'
       }
     }
     environment{
     Test_URL = "google.com"
     }

    stages {

        stage('Stage 1- Code') {
            steps {
                echo 'Hello World'
            }
        }

        stage('Stage 2- Test') {
            steps {
                echo 'Hello World'
            }
        }

        stage('Stage 3- Code Quality') {
            steps {
                echo 'Hello World'
            }
        }

        stage('Stage 4- Code Security') {
            steps {
                echo 'Hello World'
            }
        }
    }
}