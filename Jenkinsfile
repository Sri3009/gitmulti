pipeline {
    agent any
    stages {
        stage('commit tags'){
        steps{
  withCredentials([usernamePassword(credentialsId: '3025fff2-0d3f-429d-a074-5ee5ef792110', usernameVariable: 'USERNAME', passwordVariable: 'PASSWORD')]) {
  sh 'git branch'
  sh 'git branch -d child3'
  sh 'git branch'
  sh 'git branch child3'
  sh 'git branch'  
  sh 'git checkout child3'
  sh 'git checkout master'
  sh 'touch mock1'
  sh 'ls'
  sh 'git add .'
  sh 'git commit -am "This is a final commit"'
  sh 'git tag -a final3 -m "to monitor changes"'
  sh 'git push git@github.com:Sri3009/gitmulti.git master'
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

