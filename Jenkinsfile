pipeline {
    agent any
    options {
        skipStagesAfterUnstable()
    }
    stages {
        stage('Scan') {
            steps {
                git clone
                nexusPolicyEvaluation iqApplication: 'java-manifest-test-1', iqStage: 'build' , iqScanPatterns: [[scanPattern: '**/pom.xml']]
            }
        }

    }
}