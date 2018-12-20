pipeline {
   agent any
      environment {
         PATH='/usr/local/bin:/usr/bin:/bin'
      }
   stages {
      stage('NPM Setup') {
      steps {
         sh 'npm install'
      }
   }

   stages {
      stage('Build Production') {
      steps {
         sh 'ionic build browser --prod --release'
      }
   }
}