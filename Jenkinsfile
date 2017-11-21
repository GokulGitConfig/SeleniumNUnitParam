pipeline {
  agent any
  stages {
    stage('Firststep') {
      steps {
        echo 'first step done'
      }
    }
    stage('second step') {
      steps {
        git(url: 'https://github.com/GokulGitConfig/SeleniumNUnitParam.git', branch: 'master', poll: true)
      }
    }
    stage('Build') {
      steps {
        build 'dotnetbuild'
      }
    }
  }
}