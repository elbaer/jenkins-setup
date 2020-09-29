pipeline {

    agent {
        dockerfile {
            filename 'Dockerfile'
        }
    }

    options {
        timestamps()
        timeout(time: 30, unit: 'MINUTES')
        buildDiscarder(logRotator(numToKeepStr: '5'))
    }
    stages {
        stage('test') {
            steps {
                println "Hallo Welt"
            }
        }
    }
}