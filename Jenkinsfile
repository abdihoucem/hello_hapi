#!/usr/bin/env groovy

pipeline {

    agent {
        jenkins {
            image 'node'
            args '-u jenkins'
        }
    }

    stages {
        stage('Build') {
            steps {
                echo 'Building...'
                sh 'npm install'
            }
        }
        stage('Test') {
            steps {
                echo 'Testing...'
                sh 'npm test'
            }
        }
    }
}
