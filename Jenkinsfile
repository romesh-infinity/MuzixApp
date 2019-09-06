pipeline {
    agent { docker { image 'maven:latest' } }
    stages {
        stage('build') {
            when { branch 'master' }
            steps {
//                sh 'mvn clean package -DskipTests'
                sh 'mvn --version'
            }
        }
        stage('Test') {
            when { branch 'master' }
            steps {
//                sh 'mvn test'
                sh 'echo "This is test of MuzixApp"'
            }
        }
    }
}
