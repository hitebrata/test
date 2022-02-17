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

    stage('run') {
      steps {
        sh '''#!/bin/bash
echo -e "Run"'''
      }
    }

  }
  environment {
    Env = 'release'
  }
}