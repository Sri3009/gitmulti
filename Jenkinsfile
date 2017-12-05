pipeline {
    agent any
    stages {
        stage('commit tags'){
        steps{
  withCredentials([usernamePassword(credentialsId: '3025fff2-0d3f-429d-a074-5ee5ef792110', usernameVariable: 'USERNAME', passwordVariable: 'PASSWORD')]) {

  sh 'git tag -a newTagName1 -m "to monitor changes"'
  sh 'git push https://${Sri3009}:${Jersey@3009}@github.com newTagName1'
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

