pipeline {
  agent any;
  stages {
    stage('Preparing the environment') {
       steps {
          sh 'python -m pip install -r requirement.txt'
       }
    }
    stage('Code Quality') {
      steps {
        sh 'pyhton -m pylint app.py'
      }
    }
    
    stage('Tests') {
      steps {
        sh 'python -m pytest'
      }
    }
   
    stage('Build') {
      steps {
        sh 'exit 1'
      }
    }

    stage('Delivery') {
      steps {
        sh 'exit 1'
      }
    }

    stage('Deploy') {
      steps {
        sh 'exit 1'
      }
    }

  }
}
