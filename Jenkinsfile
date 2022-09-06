pipeline {
  agent any
  stages {
    stage('get project from git') {
      steps {
        git(url: 'https://github.com/YasserElassal/demo', branch: '*/master', credentialsId: '1590fb59-3ecc-4ebd-be01-ba8fb20bf543	')
      }
    }

    stage('build using maven') {
      steps {
        sh 'mvn compile package'
      }
    }

  }
}