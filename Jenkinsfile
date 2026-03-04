pipeline {
    agent any  // Use any available agent
    tools {
        gradle 'Gradle'
        jdk 'JDK'
    }
    stages {
        stage('Checkout') {
            steps {
                git branch: 'main', url: 'https://github.com/AnuragPatil3781/2023gradleapp.git'
            }
        }

        stage('Build') {
            steps {
                sh 'gradle install'  // Run Maven build
            }
        }

        stage('Test') {
            steps {
                sh 'gradle test'  // Run unit tests
            }
        }

        
        
       
        stage('Run Application') {
            steps {
                sh 'gradle run'
            }
        }

        
    }

    post {
        success {
            echo 'Build and deployment successful!'
        }
        failure {
            echo 'Build failed!'
        }
    }

}
