pipeline {
  agent any
  stages {
    stage('Inicio') {
      parallel {
        stage('Inicio') {
          steps {
            sh 'touch itworksall.ok'
            sleep(time: 10, unit: 'SECONDS')
          }
        }
        stage('continuacion') {
          steps {
            sh 'echo \'asdasd\' >> itworksall.ok'
            sleep(time: 10, unit: 'MILLISECONDS')
          }
        }
      }
    }
    stage('Phase2') {
      steps {
        echo 'We are working on $WORKSPACE'
        sh 'echo "And my Jenkins Home is $JENKINS_HOME"'
      }
    }
  }
}