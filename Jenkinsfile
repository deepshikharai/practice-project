pipeline{
  agent any
    stages {
      stage ('git') {
        steps{
          git url: 'https://github.com/deepshikharai/phptest.git'
          dir 'var/jenkins_home/workspace/DemoPipeline/phptest/PHPfinal/'
          sh 'mvn test'
            }
         }
      stage ('test') {
        agent { docker 'maven:3-alpine'}
        steps{
          dir 'var/jenkins_home/workspace/DemoPipeline/phptest/PHPfinal/'
          mvn test
        }
    }
  }
}
