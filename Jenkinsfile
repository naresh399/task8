pipeline {
   agent any
   parameters {
      choice(choices: 'Integration', description: 'Choose the environment', name: 'ENVIRONMENT')
      booleanParam(name: 'DEBUG', defaultValue: false, description: 'this is debug')
      booleanParam(name: 'DEPLOY', defaultValue: false, description: 'this is deploy')
      string(name: 'Branch   ', defaultValue: 'Default ', description: 'branch selection.')


   }
   
   stages {
       stage('Example') {
           steps {
               echo "Hello ${params.ENVIRONMENT}"
           }
       }
   }
