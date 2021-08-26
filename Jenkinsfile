pipeline {
  agent any;
  stages {
    stage('Preparing the environment') {
       steps {
          sh 'python3 -m pip install -r requirements.txt'
       }
    }
    stage('Code Quality') {
      steps {
        sh '''
                       
            python3 -m pylint app.py

           '''
      }
    }
    
    stage('Tests') {
      steps {
        sh 'python3 -m pytest'
      }
    }
   
    stage('Build') {
      steps {
        sh 'ls'
      }
    }

    stage('Delivery') {
      steps {
        sh 'echo i love linux'
      }
    }

    stage('Deploy') {
      steps {
        sh 'echo %date%'
      }
    }

  }
}
