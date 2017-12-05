pipeline {
    agent any
    stages {
        stage('checkout') {
           environment {
  GITUSER = credentials('s025fff2-0d3f-429d-a074-5ee5ef792110')
}
steps {
  sh 'git tag -a newtag -m "to monitor committed changes"'
  sh 'git push https://github.com/Sri3009/gitmulti.git newtag'
} 
        stage('end message'){
            steps{
                sh 'pwd'
                sh 'echo "done"'
            }
            
        }
    }
}

