pipeline {
  environment {
    CC = 'clang'
  }
  agent any
  stages {
    stage ('Example') {
      environment {
        DEBUG_FLAGS = '-g'
      }
      steps {
        echo "Running ${env.BUILD_ID} on ${env.JENKINS_URL}"
        
        bat 'printenv'
      }
    }
  }
}
