pipeline {
  agent {
    node {
      label 'master'
    }

  }
  stages {
    stage('') {
      steps {
        git(url: 'git@github.com:piedmont01/terraform.git', branch: 'master', credentialsId: 'jenkins')
      }
    }
  }
}