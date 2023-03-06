pipeline {
  agent any
  parameters {
    string(name: 'branch', defaultValue: 'master', description: 'Branch to build')
    booleanParam(name: 'runTests', defaultValue: true, description: 'Whether to run tests')
  }
  stages {
    stage('Build') {
      steps {
        // Build steps here
      }
    }
    stage('Test') {
      when {
        expression { params.runTests }
      }
      steps {
        // Test steps here
      }
    }
    stage('Deploy') {
      steps {
        // Deployment steps here
      }
    }
  }
}
