pipeline {
  agent any
  stages {
    stage('gitcode') {
      steps {
        git(url: 'https://github.com/saikishore789/SampleMaven.git', branch: 'main', changelog: true, poll: true)
      }
    }

    stage('maven') {
      steps {
        sh 'mvn package '
      }
    }

  }
}