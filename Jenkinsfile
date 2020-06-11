pipeline {
    agent any
     stages {
         stage ('build') {
                steps {
                withMaven(maven : 'maven_3_5_0') {
                    bat 'mvn compile'
                }
      }
    }
         stage ('deploy') {
                steps {
                withMaven(maven : 'maven_3_5_0') {
                    bat 'mvn clean deploy'
                }
            }
        }
        
    }
}
