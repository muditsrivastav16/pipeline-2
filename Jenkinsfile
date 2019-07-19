pipeline {
  environment {
    foo = "foo"
  }
  agent any
  stages {
    stage ('Example') {
      environment {
        foo2 = "foo2"
      }
      steps {
        echo "Running ${env.BUILD_ID} on ${env.JENKINS_URL}"
        
        echo " ${foo} , ${foo2}"
      }
    }
  }
}
