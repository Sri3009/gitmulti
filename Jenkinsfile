pipeline {
    agent any
    stages {
        stage('commit tags'){
        steps{
  withCredentials([usernamePassword(credentialsId: '3025fff2-0d3f-429d-a074-5ee5ef792110', usernameVariable: 'USERNAME', passwordVariable: 'PASSWORD')]) {
  sh 'git branch'
  sh 'git checkout child1'
  sh 'git checkout master'
  sh 'git tag -a finalTag -m "to monitor changes"'
  sh 'git push git@github.com:Sri3009/gitmulti.git finalTag'
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


