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
  
  parameters {
    string(name : 'name', defaultValue : 'Mr Jenkins', description : 'Hello Everyone')
    text(name :  'text' , defaultValue : '' , description : 'write some text here')
    booleanParam(name : 'toggle' , defaultValue : true, description : 'you can toggle the button')
    choice(name : 'choice' choices : ['one', 'two', 'three', 'four'], description : 'you can choose any one')
    password(name : 'password', defaultValue : 'secret' , description : 'your password is easy')
    file(name : 'file', description : 'choose file')
  }
  
  stages {
    stage ('Example') {
      environment {
        DEBUG_FLAGS = '-g'
      }
      steps {
        echo "Running ${env.BUILD_ID} on ${env.JENKINS_URL}"
        
        bat 'set'
      }
      
      steps {
        echo "${params.name}"
        echo "${params.text}"
        echo "${params.toggle}"
        echo "${params.choice}"
        echo "${params.password}"
      }
      
    }
  }
}
