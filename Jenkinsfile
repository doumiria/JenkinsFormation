pipeline {
    agent any

    parameters  {
        string(name: 'NAME', defaultValue : 'ASSIA', description: 'Your name ?')
        text(name: 'TEXT', defaultValue : 'Jenkins formation', description: 'More details...')
        booleanParam(name: 'FEMALE', defaultValue : true , description: 'Your sex?')
        choice(name: 'CHOICE', choices:['java','c++','vb'], description: 'Your language?')
        password(name:'PASSWORD',description : 'your password?')
    }
    stages {
        stage('Build'){
          steps{ 
            echo "NAME : ${ NAME }"
            echo "TEXT : ${ TEXT }"
            echo "FEMALE : ${ FEMALE }"
            echo "CHOICE : ${ CHOICE }"
            echo "PASSWORD : ${ PASSWORD }"
          }

        }
      
    }
    
}