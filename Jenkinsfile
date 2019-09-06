pipeline {
    agent { docker { image 'maven:latest' } }
    when { branch:'master' }
    stages {
        stage('build') {
            steps {
//                sh 'cd Sprint1/muzixservice ; mvn clean package -DskipTests'
                sh 'mvn --version'
            }
        }
        stage('Test') {
            steps {
//                sh 'cd Sprint1/muzixservice ; mvn test'
                sh 'echo "This is test of MuzixApp"'
            }
        }
    }
}
