pipeline {

  agent any

   options {
        buildDiscarder(logRotator(numToKeepStr: '10', artifactNumToKeepStr: '2'))
        disableConcurrentBuilds()
    }

  stages {
    stage('Hello') {

      steps {

        echo "The current time is: "

      }

    }
    stage('test') {

      steps {

        echo "test stage "

      }

    }

  }


}
