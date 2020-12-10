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
           ansiblePlaybook become: true, becomeUser: 'devops002', credentialsId: '84259fbb-0403-473e-9ae2-2d8105d57402', installation: '192.168.0.29', playbook: '/var/lib/jenkins/workspace/Ansible-Tomcat_Deployment/package_deployment/site.yaml', sudoUser: null
        }
     } 
  }
}
