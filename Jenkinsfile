pipeline {
    agent any
    stages {
        stage('checkout') {
            steps{
               
                checkout ([userRemoteConfigs: [[credentialsId: '3025fff2-0d3f-429d-a074-5ee5ef792110', url: 'https://github.com/Sri3009/gitmulti.git']]])
                }
            }    
        stage('end message'){
            steps{
                sh 'pwd'
                sh 'echo "done"'
            }
            
        }
    }
}

