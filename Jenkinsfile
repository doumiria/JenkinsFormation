
pipeline {
    agent any

   
    stages {
     stage('build')
     {
        steps {
          echo 'hello'
        }
     }
}

post{
     success
     {
       emailext (to:'jeanr@port-montreal.com',body:'test body',subject:'test subject')
     }
}

}