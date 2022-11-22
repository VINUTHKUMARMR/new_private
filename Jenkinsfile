pipeline{
  agent none
  stages{
    stage('build'){
      agent{label 'agent1'}
      steps{
        echo "this is build stage"
      }  
    }
      stage('deploy parallel'){
        parallel{
          stage('deploy_stage1'){
        agent{label 'agent2'}
      steps{
        echo "this is deploy parallel1  stage"
      }
          }
        }
      }
    
 
