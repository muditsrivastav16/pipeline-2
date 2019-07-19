pipeline {
  environment {
    CC = """${bat(
      returnStdout: true,
      script : 'echo "clang"'
    )}"""
    
    EXIT_STATUS = """${bat(
      returnStatus: true,
      script: 'exit 1'
    )}"""
  }
  agent any
  stages {
    stage ('Example') {
      environment {
        DEBUG_FLAGS = '-g'
      }
      steps {
        echo "Running ${env.BUILD_ID} on ${env.JENKINS_URL}"
        
        bat 'set'
      }
    }
  }
}
