pipeline {
    agent any
    stages {
        stage('commit tags'){
        steps{
  credentials(['3025fff2-0d3f-429d-a074-5ee5ef792110']) {

  sh 'git tag -a newtag -m "to monitor changes"'
  sh "git push origin newtag"
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

