@Library('lib-maven@master') _

pipeline {
    agent any
    stages {
        stage('Git Checkout') {
            steps {
            tache(
                branch: "master",
                url: "https://github.com/AMIBYO/maven-project.git"
            )
            }
    }
       stage('Maven') {
            steps {
           notification type: "slack", message: "Build succeeded"
            }
    }
    }
}
