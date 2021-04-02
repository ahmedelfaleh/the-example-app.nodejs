pipeline {
  agent any
  stages {
    stage("npm install") {
      steps {
        echo "excuting npm"
        nodejs('node-8.0.0')
          sh 'npm install'
      }
    }
    stage("npm run") {
      steps {
        echo "npm run"
        nodejs('node-8.0.0')
          sh 'npm run start:dev'
      }
    }
  }
}
