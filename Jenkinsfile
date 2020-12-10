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
           ansiblePlaybook become: true, becomeUser: 'devops002', installation: '192.168.0.29', playbook: '/var/lib/jenkins/workspace/Ansible-Tomcat_Deployment/package_deployment/'
        }
     } 
  }
}
