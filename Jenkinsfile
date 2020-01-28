pipeline{
  agent any
    stages {
      stage ('git') {
        steps{
          git url: 'https://github.com/deepshikharai/phptest.git'
            }
         }
      stage ('test') {
        steps{
          dir '$WORKSPACE/DemoPipeline/phptest/PHPfinal/'
          mvn test
        }
    }
  }
}
