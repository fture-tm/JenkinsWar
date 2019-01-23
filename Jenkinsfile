pipeline {
    agent { docker 'maven:3.3.3' }
    stages {
                stage ('Testing Stage') {

            steps {
                withMaven(maven : 'maven_3_5_0') {
                    sh 'mvn test'
                }
            }
        }
        stage('build') {
            steps {
                bat 'mvn --version'
            }
        }
    }
}
