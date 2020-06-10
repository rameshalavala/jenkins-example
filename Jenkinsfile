pipeline {
    agent any
     stages {
        stage('Checkout') {
           steps {
            git 'https://github.com/rameshalavala/jenkins-example'
      }
    }
         stage ('build') {
                steps {
                withMaven(maven : 'maven_3_5_0') {
                    sh 'mvn clean'
                }
            }
        }
        
    }
}
