pipeline {
    agent {
        label 'maven'
    }
    stages {
        stage('stage1') {
            steps {
                sh """
                    mvn -version
                """
            }
        }
        stage('stage2') {
            steps {
                sh """
                    oc version
                    oc whoami
                    oc get pods -n jenkins
                """
            }
        }
    }
}

