pipeline {
  agent any

  stages {
    stage('Build') {
      steps {
        echo 'Building the project...'
        sh 'pwd'
        sh 'ls'
        sh 'mvn clean install'
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
