pipeline {
    agent { docker { image 'maven' } }
    stages {
        stage('build') {
            steps {
                sh 'cd Sprint1/muzixservice ; mvn clean package -DskipTests'
            }
        }
        stage('Test') {
            steps {
                sh 'cd Sprint1/muzixservice ; mvn test'
            }
        }
    }
}
