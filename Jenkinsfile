pipeline {
   agent any
    stages {
      stage('SCM Checkout') {
         steps {
            git 'https://github.com/prashanticoder/simple-java-maven-app.git'
        }
    }
    stage ('Build') {
        steps {
            sh '/opt/maven/bin/mvn clean verify -Dmaven.test.skip=true'
        }
    }
}
}
