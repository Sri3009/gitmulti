pipeline {
    agent any
    stages {
        stage('commit tags'){
        steps{
  withCredentials([usernamePassword(credentialsId: '3025fff2-0d3f-429d-a074-5ee5ef792110', usernameVariable: 'USERNAME', passwordVariable: 'PASSWORD')]) {
  sh 'git tag -a final2 -m "to monitor changes"'
  sh 'git branch'
  sh 'git push git@github.com:Sri3009/gitmulti.git child2' 
  sh 'git push git@github.com:Sri3009/gitmulti.git final2'
  }
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

