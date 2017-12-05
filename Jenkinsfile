pipeline {
    agent any
    stages {
        stage('commit tags'){
        steps{
  withCredentials([usernamePassword(credentialsId: '3025fff2-0d3f-429d-a074-5ee5ef792110', usernameVariable: 'USERNAME', passwordVariable: 'PASSWORD')]) {
echo "$USERNAME"
  //sh 'git tag -a newTagName3 -m "to monitor changes"'
  //sh 'git push https://github.com/Sri3009/gitmulti.git newTagName3'
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

