pipeline {
    agent any
    environment {
    PATH= "/opt/maven/bin:$PATH"
    }
    stages {
        stage("clonig stage"){
            steps{
                git branch: 'main', url: 'https://github.com/Adv-kishore/Groovy.git'
            }
        }
        stage("Building stage"){
            steps{
                sh "mvn clean install"
            }
        }  
    }
}
