pipeline { 
    agent any 
    options {
        skipStagesAfterUnstable()
    }
    stages {
        stage('Build') { 
            steps { 
                sh "echo `whoami`"
                sh "echo `pwd`"
                sh "mvn clean initialize package -f *.application.parent/pom.xml"
            }
        }
    }
}