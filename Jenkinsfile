pipeline {
  agent any
  def name = 'mudit'
  stages {
    stage ('Example') {
      steps {
        echo "Running ${env.BUILD_ID} on ${env.JENKINS_URL}"
        echo "name is ${name}"
      }
    }
  }
}
