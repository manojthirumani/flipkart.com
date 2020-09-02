pipeline {
    agent any

    stages {
        stage('gitcheckout') {
            steps {
                checkout([$class: 'GitSCM', branches: [[name: '*/master']], doGenerateSubmoduleConfigurations: false, extensions: [], submoduleCfg: [], userRemoteConfigs: [[credentialsId: 'Githubconnection', url: 'https://github.com/manojthirumani/flipkart.com.git']]])
            }
        }
        stage('buildstage') {
            steps {
            echo 'building project'    
                } }
                stage('teststage') {
            steps {
            echo 'testing project'    
               } }
         stage('deplyomentstage') {
            steps {
            echo 'deployment project'    
                } }
                stage('monitorstage') {
            steps {
            echo 'monitoring project'    
               } }
                    
                }
    }
