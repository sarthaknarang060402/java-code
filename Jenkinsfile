pipeline{
    agent any

    stages {
        stage('GIT CHECKOUT'){
            steps{
                git branch: 'main', url: 'https://github.com/sarthaknarang060402/java-code'
            }
        }
        stage('UNIT TESTING') {
            steps {
                sh 'mvn test'
            }
        }
        stage('INTEGRATION TESTING') {
            steps {
                sh 'mvn verify -DskipUnitTests'
            }
        }
    }
    
}
