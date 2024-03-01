pipeline {
    agent any

    parameters{
      booleanParam(name: 'DEPLOY_TO', defaultValue:false, description: 'production ?'  )
    }

    stages {
        stage('Build'){
          steps{ 
            echo 'Build !'
          }
        }

         stage('Deployement production'){
          
          when{ 
            anyOf{
            branch 'masterX'
            expression { params.DEPLOY_TO}
            }
          }

          steps{ 
            echo 'Deploy !'
          }
        }
    }
    
}