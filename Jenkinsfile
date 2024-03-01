pipeline {

  agent any

  options {

    buildDiscarder logRotator(artifactDaysToKeepStr: '', artifactNumToKeepStr: '5', daysToKeepStr: '', numToKeepStr: '5')

  }

  stages {
    stage('Hello') {

      steps {

       sh 'current_time=$(date +"%T")'
        echo "The current time is: ${current_time}"

      }

    }

  }

}
