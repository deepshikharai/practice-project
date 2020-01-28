pipeline{
  agent any
    stages {
      stage ('git') {
        steps{
          git url: 'https://github.com/deepshikharai/phptest.git'
            }
         }
      stage ('Test') {
        steps{
          sh 'mvn test'
        }
    }
  }
}
