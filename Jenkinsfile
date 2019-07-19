pipeline {
  agent any
  stages {
    stage ('Example') {
      steps {
        echo "Running ${env.BUILD_ID} on ${env.JENKINS_URL}"
        def name = 'mudit'
        bat echo "name is ${name}"
      }
    }
  }
}
