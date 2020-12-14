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
          sh "sudo ansible-Playbook '/var/lib/jenkins/workspace/Ansible-Tomcat_Deployment/package_deployment/site.yaml"
          //ansiblePlaybook credentialsId: 'private_key', inventory: 'dev.inv', playbook: 'site.yaml'
          
        }
     } 
  }
}
