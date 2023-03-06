pipeline {
  agent {
    name 'JenkinsAgent1'
  }
  parameters {
    string(name: 'branch', defaultValue: 'master', description: 'Branch to build')
    booleanParam(name: 'runTests', defaultValue: true, description: 'Whether to run tests')
  }
  stages {
    stage('Build') {
      steps {
        sh 'echo "Build"'
      }
    }
    stage('Test') {
      when {
        expression { params.runTests }
      }
      steps {
        sh 'echo "Test"'
      }
    }
    stage('Deploy') {
      steps {
        sh 'echo "Deploy"'
      }
    }
  }
}
