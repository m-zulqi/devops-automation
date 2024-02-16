pipeline {
  agent any
  tools {
    maven 'Maven-3.8.4'
  }

  stages {
    
    stage('Build Maven') {
      steps {
        checkout scmGit(branches: [[name: '*/main']], extensions: [], userRemoteConfigs: [[url: 'https://github.com/m-zulqi/devops-automation']])
        sh 'mvn clean install'  
      }
    }
    
  }
  
}
