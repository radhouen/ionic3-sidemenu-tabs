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

   stage('IOS Build') {
   steps {
      sh 'ionic cordova build ios'
     } 
  }

   stage('Android Build') {
   steps {
      sh 'ionic cordova build android'
   }
  }
}
}
