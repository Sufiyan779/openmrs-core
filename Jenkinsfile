pipeline{
    agent {label 'OPENJDK-11-1'}
    triggers{
        pollSCM('30 22 * *  *')
    }
 stages{
    stage('pull from vcs') {
        steps{
            git url: 'https://github.com/Sufiyan779/openmrs-core.git',
            branch: 'SPRINT_1_DEV'
        }

    }
    stage('build'){
        steps{
            sh 'mvn package'
        }
    }
 }   
}