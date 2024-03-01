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
            allOf{
            branch 'master'
            environment name : 'DEPLOY_TO',value : 'production'
            }
          }

          steps{ 
            echo 'Deploy !'
          }
        }
    }
    
}