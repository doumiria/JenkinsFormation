
pipeline {
    agent any

    tools {
      gradle 'Gradle8.7'
      nodejs 'NodeJs21.6.2'
    }
    stages {
     stage('build')
     {
        steps {
          sh 'gradle -v'
          sh 'node -v'
        }
     }
}

}