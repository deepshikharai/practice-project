pipeline{
  agent any
    stages {
      stage ('git') {
        steps{
          git url: 'https://github.com/deepshikharai/phptest.git'
            }
         }
      stage ('Test') {
        agent { docker 'maven:3-alpine'}
        steps{
          sh 'mvn test'
        }
    }
  }
}
