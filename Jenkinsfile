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
           //ansiblePlaybook installation: 'Ansible', inventory: 'webserver', playbook: 'site.yaml'
           ansiblePlaybook installation: 'Ansible', inventory: 'webserver', playbook: '/workspace/Ansible-Tomcat_Deployment/package_deployment'
        }
     } 
  }
}
