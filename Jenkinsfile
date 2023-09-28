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

     options {
             ansiColor('xterm')
         }
     parameters {
        string(name: 'PERSON', defaultValue: 'Mr Jenkins', description: 'Who should I say hello to?')

        text(name: 'BIOGRAPHY', defaultValue: '', description: 'Enter some information about the person')

        booleanParam(name: 'TOGGLE', defaultValue: true, description: 'Toggle this value')

        choice(name: 'CHOICE', choices: ['One', 'Two', 'Three'], description: 'Pick something')

        password(name: 'PASSWORD', defaultValue: 'SECRET', description: 'Enter a password')
    }
    stages {

        stage('Stage 1- Code') {
            steps {
                echo 'Hello World Stage-1'
                echo Test_URL
                echo SSH
                sh 'env'
                sh 'ansible -i 172.31.23.36, all -e ansible_user=${SSH_USR} -e ansible_password=${SSH_PSW} -m ping'
                sh 'mvn version'


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