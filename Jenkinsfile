pipeline {
    agent any

    stages {
        stage('Build with Maven') {
            agent {
                docker { 
                    image 'maven:3.8.1-adoptopenjdk-11' 
                }
            }
            steps {
                // Your Maven build steps here
		sh 'hello maven'
            }
        }

        stage('Build with Node.js') {
            agent {
                docker {
                    image 'node:16-alpine'
                }
            }
            steps {
                // Your Node.js build steps here
		sh 'hello nodejs'
            }
        }
    }
}
