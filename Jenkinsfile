pipeline{
  agent { label 'nodejs10' }
  stages{
    stage ('checkout'){
      steps {
        deleteDir()
        checkout([$class: 'GitSCM', branches: [[name: '*/develop']], doGenerateSubmoduleConfigurations: false, extensions: [], submoduleCfg: [], userRemoteConfigs: [[credentialsId: 'jenkins-github-credentials', url: 'git@github.com:nadafly0815/daas5th-music.git']]])
      }
    }
  }
}
