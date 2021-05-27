pipeline {
    agent any
    options {
        skipStagesAfterUnstable()
    }
    stages {
        stage('Scan') {
            steps {
                git clone
                nexusPolicyEvaluation iqApplication: 'java-manifest-test-1', iqScanPatterns: [[scanPattern:  '**/pom.xml' ], [scanPattern:  '**/build.gradle']], iqStage: 'build'
            }
        }

    }
}