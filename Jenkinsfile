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
    stage('Run Ansible Playbook') {
            steps {
                script {
                    // Run Ansible playbook
                    sh 'ansible-playbook -i inventory install_nginx.yml'
                }
            }
        }

  }


}
