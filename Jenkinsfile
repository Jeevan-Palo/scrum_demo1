pipeline {
  agent {
    docker {
      image 'cypress/included:9.4.1'
      args '-p 3000:3000'
    }
  }

  stages {
    stage('Build and Test') {

      steps {
        // sh 'npm ci'
        // sh "npm run test:ci:record"
        sh 'npm install'
        sh 'npx cypress run'
      }
    }
  }
}
