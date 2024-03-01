pipeline {
    agent any

    options{
      parallelsAlwaysFailFast()
    }

    stages {
        stage('Build'){
          //failFast true
          parallel{ 
           stage('Build frontend'){
                  steps{ 
                    echo 'Build frontend !'
                  }
                }

            stage('Build backend'){
                  steps{ 
                    echo 'Build backend !'
                  }
                }    
          }
        }

         stage('Deployement production'){
          steps{ 
            echo 'Deploy !'
          }
        }
    }
    
}