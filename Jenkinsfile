pipeline {
    agent any

    stages {
        stage('Build and test'){
          
          matrix{ 
           axes {
            axis {
              name 'PLATFORM'
              values 'linux','macos','windows'
            }

              axis {
              name 'BROWSER'
              values 'firefox','chrome','safari'
            }

           }
          }
        stages {
                stage('build'){
                  steps{ 
                    echo 'Construire pour ${ PLATFORM} -  ${ BROWSER}!'
                  }
                }

                 stage('test'){
                  steps{ 
                    echo 'Test pour ${ PLATFORM} -  ${ BROWSER}!'
                  }
                }
        }
        
    }
    }   
}