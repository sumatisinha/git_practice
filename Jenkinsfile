pipeline {
  agent any 
  stages {
    stage('Checkout Source Code') {
      steps {
        echo 'Sharting Git checkout...'
        git url: 'https://github.com/sumatisinha/git_practice.git', branch: 'main'
        echo 'Git checkout completed.'
      }
    }
    stage('Run Example Command') {
      steps {
        echo 'Executing some commands...'
        bat 'echo "Hellooo from declarativ pipeline!"'
        bat 'echo --- Reading README ----'
        bat 'type README.md'
      }
    }
  }
}
