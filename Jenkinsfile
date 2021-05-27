pipeline {
    agent any

    stages {
        stage('Scan Build') {
            steps {
                nexusPolicyEvaluation iqApplication: 'java-manifest-test-1', iqScanPatterns: [[scanPattern:  '**/pom.xml' ], [scanPattern:  '**/build.gradle']], iqStage: 'build'
            }
        }

    }
}