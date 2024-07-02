pipeline {
  agent {
    node { label 'workstation'}
  }

  stages {

    stage('Unit Test ') {
          steps {
            echo 'Unit Test'
          }
    }

    stage('Code Analysis ') {
          steps {
            sh 'sonar-scanner -Dsonar.host.url=http://52.55.243.127:9000 -Dsonar.login=admin -Dsonar.password=admin123 -Dsonar.projectKey=frontend -Dsonar.qualitygate.wait=true'
          }
    }

    stage('Security scan ') {
          steps {
            echo 'Security scan'
          }
    }
    
    stage('Publish Artifact ') {
          steps {
            echo 'Publish Artifact'
          }
    }

  }

}