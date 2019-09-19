pipeline{
    agent { label 'slave1' }
    stages{
        stage('build'){
            steps{
                sh 'sudo apt-get install maven'
                sh 'mvn clean package'
            }
        }
    }
}
