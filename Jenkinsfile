pipeline {
    agent any
    stages {
        stage('checkout') {
            steps{
               git url: "git@github.com:Sri3009/gitmulti.git",
               credentialsId: '3025fff2-0d3f-429d-a074-5ee5ef792110',
    branch: newtestbranch
sh 'git tag -a testtag -m "testing file"'
sh 'git merge newtestbranch'
sh 'git commit -am "Merged newtestbranch branch to master'
sh 'git push origin master'
            }    
            
        }
    }
}

