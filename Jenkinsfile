pipeline {
    agent any
    options {
        skipStagesAfterUnstable()
    }
    stages {
        stage('Scan') {
            steps {
                git clone
                nexusPolicyEvaluation advancedProperties: '', enableDebugLogging: false, failBuildOnNetworkError: false, iqApplication: selectedApplication('java-manifest-test-1'), iqScanPatterns: [[scanPattern: 'pom.xml']], iqStage: 'build', jobCredentialsId: ''
            }
        }

    }
}