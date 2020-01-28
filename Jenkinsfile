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
         
          mvn test
        }
    }
  }
}
