
// to komewntarz
pipeline {
    agent { label 'glowne' }
    environment {
       PATH="/bin:/sbin:/usr/bin"
    }
    stages {
        stage('check pips') {
            steps {
            // epel wymagane do pip
            sh 'yum -y install epel-release'
            sh 'yum -y install python-pip'
            sh 'yum -y install centos-release-scl'
            sh 'yum -y install rh-python36'
            // enable p3 w bashu  nie wiem czy permanentnie
            sh 'scl enable rh-python36 bash'
            sh 'python --version'
            sh 'pip3 install awscli --upgrade --user'
            sh 'python -m ensurepip"
            sh 'aws --version'
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


