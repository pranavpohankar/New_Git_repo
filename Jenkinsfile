pipeline {
  agent any

  environment {
    APP_ENV = 'staging'
  }

  stages {
    stage('Build') {
      steps {
        echo 'Step 1: Building the application...'
        sh 'df -PhT
        sh 'pwd'
        sh 'ls -l'
      }
    }

    stage('Test') {
      steps {
        echo 'Step 2: Running tests...'
        sh 'echo Running dummy tests...'
      }
    }

    stage('Deploy') {
      steps {
        echo "Step 3: Deploying to ${APP_ENV}..."
        sh 'echo Deploying application...'
      }
    }
  }

  post {
    success {
      echo '✅ Pipeline completed successfully.'
    }
    failure {
      echo '❌ Pipeline failed.'
    }
  }
}
