pipeline {
  agent { label 'agent2' }
  stages {
    stage('build') {
      steps {
        sh 'pip install -r requirements.txt'
      }
    }
    stage('test') {
      steps {
        sh 'python3 main.py -env prod -i smoke -t ./tests -n 1'
      }   
    }
  }
}
