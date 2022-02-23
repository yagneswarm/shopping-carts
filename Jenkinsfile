pipeline {
  agent any
  stages {
    stage('shopping-carts-build') {
      steps {
        echo 'this is the build job'
        sh 'mvn compile'
      }
    }

    stage('shopping-carts-test') {
      steps {
        echo 'this is the test job'
        sh 'mvn test'
      }
    }

    stage('shopping-carts-package') {
      steps {
        echo 'this is the package job'
        sh 'mvn package'
      }
    }


  }
  tools {
    maven 'maven'
  }
  post {
    always {
      echo 'this pipeline has completed...'
    }

  }
}
