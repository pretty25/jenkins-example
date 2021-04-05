pipeline {
  agent {
   // label 'docker-slave'
   label 'java11-maven'
  }
    stages {
        stage ('Compile Stage') {
            steps {
                    sh 'mvn clean compile'
                }
            }
        stage ('Testing Stage') {
            steps {
                    sh 'mvn test'
                }
            }
        stage ('Deployment Stage') {
            steps {
                    sh 'mvn deploy'
                }
            }
    }
}
