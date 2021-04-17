pipeline{
  agent any
    stages{
      stage ('ssh-test'){
        steps{
          sshagent(['3eaf4b4a-3aa7-4c04-806e-e33567e15c13']){
            bat 'ssh -o StrictHostKeyChecking=no ubuntu@3.128.155.28 pwd'
            bat 'scp -r C:/WINDOWS/system32/config/systemprofile/AppData/Local/Jenkins/.jenkins/workspace/practice ubuntu@3.128.155.28:/home/ubuntu/artifacts'
            }
            }
            }
            }
            }
  
