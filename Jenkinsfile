pipeline{
  agent { label 'nodejs8' }
  stages{
    stage ('checkout'){
      steps {
        sh '''
          echo "checkout!"
        '''
      }
    }
    stage ('install modules'){
      steps{
        sh '''
          echo "install modules!"
        '''
      }
    }
    stage ('test'){
      steps{
        sh '''
          echo "test!"
        '''
      }
    }
    stage ('code quality'){
      steps{
          echo "code quality!"
      }
    }
    stage ('build') {
      steps{
          echo "build!"
      }
    }
    stage ('build image') {
      steps{
        sh '''
          echo "build image!"
        '''
      }
    }
  }
}
