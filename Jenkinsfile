@Library('jenkins-shared-library') _

pipeline {
  agent any

  stages {
    stage('Clone Repository') {
      steps {
        git url: 'https://github.com/Juhi5863/jenkins-shared-library2.git', branch: 'main'
      }
    }

    stage('Build') {
      steps {
        sh 'echo "Building the application"'
      }
    }

    stage('Running Shared Library') {
      steps {
        script {
          commonBuild() 
        }
      }
    }
  }
}
