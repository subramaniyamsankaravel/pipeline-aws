pipeline{
  agent any
    stages{
      stage ('ssh-test'){
        steps{
          sshagent(['cc92063a-d88c-46eb-a70a-f6f376fa33fa']){
            bat 'ssh -o StrictHostKeyChecking=no ubuntu@52.15.182.190 pwd'
            bat 'scp -r /var/jenkins_home/workspace/pipeline-challenge/calculator/target/calculator-0.0.1-SNAPSHOT.jar ubuntu@52.15.182.190:/home/ubuntu/artifacts'
            }
            }
            }
            }
            }
  
