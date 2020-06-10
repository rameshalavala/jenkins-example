pipeline {
    agent any
stage('Checkout') {
      steps {
        git 'https://github.com/rameshalavala/jenkins-example'
      }
    }
    stages {
        stage ('build') {

            steps {
                withMaven(maven : 'maven_3_5_0') {
                    bat 'mvn clean'
                }
            }
        }
        
    }

}
