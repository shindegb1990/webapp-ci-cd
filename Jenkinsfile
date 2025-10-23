pipeline {
    agent any
    triggers {
      cron( 'H H * * 0')
    }
    stages {
    stage('Build'){
    steps {
     sh 'mvn clean install'
      }
    }
    stage('Test'){
        steps {
         sh 'mvn test'
          }
        }
    stage('Deploy'){
    steps{
    echo 'Deploying application....'
    }
   }
  }
 }
