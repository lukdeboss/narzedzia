
// to komewntarz
pipeline {
    agent { label 'glowne' }
    environment {
       PATH="/bin:/sbin:/usr/bin"
    }
    stages {
        stage('check pips') {
            steps {
            sh 'yum install epel-release'
            sh 'yum install python-pip'
            sh 'python --version'
            sh 'pip --version'
            sh 'pip3 --version'
            }
        }
        stage('instalacja ansible') {
            steps {
                echo 'instalacja ansible'
            }
        }
        stage('Test') {
            steps {
                echo 'Testing..'
            }
        }
        stage('Deploy') {
            steps {
                echo 'Deploying....'
            }
        }
    }
}


