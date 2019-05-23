pipeline {
  agent {
    node {
      label 'master'
    }

  }
  stages {
    stage('error') {
      steps {
        git(url: 'git@github.com:piedmont01/terraform.git', branch: 'master', credentialsId: 'jenkins')
      }
    }
    stage('plan') {
      steps {
        sh 'terraform init'
      }
    }
  }
}