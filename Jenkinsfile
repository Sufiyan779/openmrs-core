Pipeline{
    Agent {label 'OPENJDK-11-1'}
 Stages{
    Stage('pull from vcs') {
        steps{
            git url: 'https://github.com/Sufiyan779/openmrs-core.git',
            branch: 'SPRINT_1_DEV'
        }

    }
    Stage('build'){
        steps{
            sh 'mvn package'
        }
    }
 }   
}