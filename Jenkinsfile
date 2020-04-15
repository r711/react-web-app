pipeline
{
  agent any
  
  tools
  {
  nodejs 'node'
  }
  
  stages
  {
    stage('Build')
    {
      steps 
      {
        script
        {
          checkout changelog: false, poll: false, scm: [$class: 'GitSCM', branches: [[name: '*/master']], doGenerateSubmoduleConfigurations: false, extensions: [], submoduleCfg: [], userRemoteConfigs: [[url: 'https://github.com/r711/react-web-app.git']]]      
        }
      }
    }
  }
}
