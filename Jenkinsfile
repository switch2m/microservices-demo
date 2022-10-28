pipeline {
    agent any
    stages {
        stage('build image') {
            steps {
                echo 'Building the image'
                withCredentials([usernamePassword(credentialsId: 'docker-hub-repo', passwordVariable: 'PASS', usernameVariable: 'USER')]) {
                    sh 'pwd'
                    sh 'ls'
                    //sh "docker build -t micro-app/:${BUILD_NUMBER} ."
                    //sh "echo $PASS | docker login -u $USER --password-stdin"
                    //sh "docker push beamtel/web:${BUILD_NUMBER}"
                }
            }
        }
    }
}
