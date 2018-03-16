pipeline {
  agent any
  stages {
    stage('hello') {
      parallel {
        stage('hello') {
          steps {
            echo 'hello'
          }
        }
        stage('error') {
          steps {
            sh '''echo drink tea
1


'''
          }
        }
      }
    }
    stage('goodbye') {
      parallel {
        stage('goodbye') {
          steps {
            echo 'goodbye'
            sh 'echo goodbye'
          }
        }
        stage('error') {
          steps {
            sh 'echo that was a nice cup of tea 2'
          }
        }
      }
    }
  }
}
