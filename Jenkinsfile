pipeline { 
    agent any 
    options {
        skipStagesAfterUnstable()
    }
    stages {
        stage('Build') { 
            steps { 
                sh "mvn clean initialize package -f *.application"
            }
        }
    }
}