
pipeline {
    agent any

    tools {
      gradle 'Gradle8.7'
    }
    stages {
     stage('build')
     {
        steps {
          sh 'gradle -v'
        }
     }
}

}