pipeline {
    agent any  // Use any available agent

    tools {
        gradle 'Gradle'
        jdk 'JDK'
=======

    tools {
        maven 'Maven'  // Ensure this matches the name configured in Jenkins
>>>>>>> 5b6e52c8d743bc91213661fb4b958e12d0b6f483
    }
    stages {
        stage('Checkout') {
            steps {
<<<<<<< HEAD
                git branch: 'main', url: 'https://github.com/AnuragPatil3781/2023gradleapp.git'
=======
                git branch: 'master', url: 'https://github.com/AnuragPatil3781/mavenhello.git'
>>>>>>> 5b6e52c8d743bc91213661fb4b958e12d0b6f483
            }
        }

        stage('Build') {
            steps {
<<<<<<< HEAD
                sh 'gradle install'  // Run Maven build
=======
                sh 'mvn clean package'  // Run Maven build
>>>>>>> 5b6e52c8d743bc91213661fb4b958e12d0b6f483
            }
        }

        stage('Test') {
            steps {
<<<<<<< HEAD
                sh 'gradle test'  // Run unit tests
=======
                sh 'mvn test'  // Run unit tests
>>>>>>> 5b6e52c8d743bc91213661fb4b958e12d0b6f483
            }
        }

        
        
       
        stage('Run Application') {
            steps {
<<<<<<< HEAD
                sh 'gradle run'
=======
                // Start the JAR application
                sh 'java -jar target/ mavenlistapp-1.0-SNAPSHOT.jar'
>>>>>>> 5b6e52c8d743bc91213661fb4b958e12d0b6f483
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
<<<<<<< HEAD

}

=======
}
>>>>>>> 5b6e52c8d743bc91213661fb4b958e12d0b6f483
