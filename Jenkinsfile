pipeline {
  agent any
  stages {
    stage('Checkout code') {
      steps {
        git(url: 'https://github.com/sumit8340/python_flask_app', branch: 'main')
      }
    }

    stage('Build') {
      steps {
        sh '''sudo docker build -f Dockerfile .
'''
      }
    }

  }
}