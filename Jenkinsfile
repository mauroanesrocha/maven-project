pipeline{
    agent { label 'slave1' }
    stages{
        stage('build'){
            steps{
                sh 'sudo apt-get install maven -y'
                sh 'mvn clean package'
                sh "docker build . -t tomcatwebapp:${env.BUILD_ID}"
            }
        }
    }
}
