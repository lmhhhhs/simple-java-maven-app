pipeline {
  agent {
    docker {
      args '-v /Users/liminghui/m2:/root/.m2 --privileged=true'
      image 'maven:3.6.1-alpine'
    }

  }
  stages {
    stage('Build') {
      steps {
        sh 'mvn -B -DskipTests clean package'
      }
    }

  }
}