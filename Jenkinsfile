pipeline {
  agent any
  stages {
    stage('C8.6MN Trigger') {
      parallel {
        stage('C8.6MN Trigger') {
          steps {
            bat 'c8.6MN.bat'
          }
        }
        stage('C8.6RM_Trigger') {
          steps {
            bat 'c8.6RM.bat'
          }
        }
      }
    }
    stage('c8MN_Trigger') {
      parallel {
        stage('c8MN_Trigger') {
          steps {
            bat 'c8MN.bat'
          }
        }
        stage('c8RM_Trigger') {
          steps {
            bat 'c8RM.bat'
          }
        }
      }
    }
  }
}