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
            allOf{
            branch 'master'
            equals expected:true, actual : params.DEPLOY_TO
            }
          }

          steps{ 
            echo 'Deploy !'
          }
        }
    }
    
}