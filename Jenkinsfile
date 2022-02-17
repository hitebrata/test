pipeline {
  agent any
  stages {
    stage('CodeBuild') {
      steps {
        publishChecks()
        sh '''#!/bin/bash
echo -e "Hello"'''
      }
    }

  }
  environment {
    Env = 'release'
  }
}