pipeline {
    agent any

    stages {
        stage('Build'){
          steps{ 
            echo 'Build !'
          }
        }

         stage('Deployement production'){
          
          when{ 
            branch 'master'
          }

          steps{ 
            echo 'Deploy !'
          }
        }
    }
    
}