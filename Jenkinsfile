pipeline{
  agent {
    docker {
      image 'maven:3.6.3-jdk-11'
    }
  }
    stages{
      stage ('ssh-test'){
        steps{
          sshagent(['4caf8f9d-4507-4358-a814-4a2866505100']){
            sh 'ssh -o StrictHostKeyChecking=no ubuntu@18.216.159.12 pwd'
            sh 'scp -r /var/jenkins_home/workspace/pipeline-challenge/calculator/target/calculator-0.0.1-SNAPSHOT.jar ubuntu@18.216.159.12:/home/ubuntu/artifacts'
            }
            }
            }
            }
            }
  
