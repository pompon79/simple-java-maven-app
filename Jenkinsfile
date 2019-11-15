pipeline {
  agent any
  stages {
    stage('get repo') {
      steps {
        git(url: 'https://github.com/jenkins-docs/simple-java-maven-app.git', branch: 'master')
      }
    }

    stage('Build') {
      steps {
        sh 'mvn -B -DskipTests clean package'
      }
    }

    stage('finish') {
      steps {
        echo 'YO!'
      }
    }

  }
}