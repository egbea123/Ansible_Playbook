def workspace
pipeline 
{
  agent any
  stages {
    stage('checkout') {
           steps {    
                git branch: 'master', url: 'https://github.com/egbea123/Ansible_Playbook.git'
          }
     }
     stage('Ansible Deploy')
     {    
        steps 
        { 
           ansiblePlaybook credentialsId: '18e7ceb4-dc87-49aa-9dc3-a071ce6be8c1', installation: 'ansible_server', playbook: 'site.yaml'
        }
     } 
  }
}
