pipeline {
  agent any

  stages {
    stage('Checkout') {
      steps {
        checkout scm
      }
    }

    stage('Build') {
      steps {
        echo 'Building the project...'
        // Replace with your build tool command:
        // sh 'mvn clean install'
        // or: sh 'npm install'
      }
    }

    stage('Test') {
      steps {
        echo 'Running tests...'
        // sh 'mvn test' or sh 'npm test'
      }
    }

    stage('Deploy') {
      steps {
        echo 'Deploying application...'
        // sh './deploy.sh' or your deployment logic
      }
    }
  }

  post {
    success {
      echo 'Build completed successfully.'
    }
    failure {
      echo 'Build failed.'
    }
  }
}
