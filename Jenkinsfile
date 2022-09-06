pipeline {
  agent any
  stages {
    stage('echo') {
      steps {
        bat 'echo "yasser"'
      }
    }

    stage('git') {
      steps {
        git(url: 'https://github.com/YasserElassal/demo', branch: 'master', credentialsId: 'myGithub')
      }
    }

    stage('build') {
      steps {
        sh 'mvn compile package'
      }
    }

  }
}