pipeline {
    agent any  // Allows Jenkins to choose any available agent to run the pipeline

    stages {
        // Stage 1: Checkout
        stage('Checkout') {
            steps {
                git branch: 'main', url: 'https://github.com/himanshu930/devops-069.git' // Replace with your actual repository URL
            }
        }

        // Stage 2: Build
        stage('Build') {
            steps {
                sh 'javac GitJavaFile.java' // Replace with your actual Java file name
            }
        }

        // Stage 3: Run
        stage('Run') {
            steps {
                sh 'java GitJavaFile' // Replace with your actual class name
            }
        }
    }
}
