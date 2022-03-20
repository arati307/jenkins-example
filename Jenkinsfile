pipeline {
    agent any
    tools { 
        maven 'Maven 3.8.5' 
        jdk 'jdk9'

    stages {
        stage ('Compile Stage') {

            steps {
                withMaven(maven : 'maven 3.8.5') {
                    sh 'mvn clean compile'
                }
            }
        }

        stage ('Testing Stage') {

            steps {
                withMaven(maven : 'maven 3.8.5') {
                    sh 'mvn test'
                }
            }
        }



        }
    }
}
