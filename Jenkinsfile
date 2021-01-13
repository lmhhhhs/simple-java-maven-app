pipeline {
  agent {
    docker {
      image 'maven:3.3.3'
      args '-v /Users/liminghui/m2:/root/.m2 --privileged=true'
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