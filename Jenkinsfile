pipeline {
    agent any

    stages {
        stage('Build'){
          steps{ 
            echo 'Build !'
          }
        }

         stage('Deployement production'){
          input { 
           message 'Voulez-vous deployer en production ?'
           ok 'deployer !'
           submitter 'admin,devops'
           submitterParameter 'USER_SUBMIT'
           parameters { 
             string(name: 'VERSION', defaultValue: 'latest', description: 'une version')
           }
          }
          steps{ 
            echo "user : ${ USER_SUBMIT }"
            echo "version : ${ VERSION }"
            echo 'Deploy !'
          }
        }
    }
    
}