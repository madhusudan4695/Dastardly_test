pipeline {
    agent {
        docker { image 'node:16.13.1-alpine' }
    }
    stages {
        stage('Test') {
            steps {
                sh 'node --version'
            }
        }
    }
}
      steps {
        // Steps run in node:7-alpine docker container on docker agent
        sh 'node --version'
      }
    }
    
    stage('Docker maven test') {
      agent {
        docker {
          image 'maven:3-alpine'
        }
      }
      steps {
        // Steps run in maven:3-alpine docker container on docker agent
        sh 'mvn --version'
      }
    }
  }
}
