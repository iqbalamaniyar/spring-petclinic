pipeline {
    agent { label 'mvn' }
    stages {
        stage('vcs') {
            steps {
            git url: 'https://github.com/spring-projects/spring-petclinic.git',
                branch: 'main'
            }
        }   
        stage('build') {
            steps {
                sh 'mvn package'
            }
        }
    }
}
