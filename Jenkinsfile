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
           //sh "cd /var/lib/jenkins/workspace/Ansible-Tomcat_Deployment/package_deployment/"
           //sh  "ansible-playbook site.yaml"
           ansiblePlaybook become: true, becomeUser: 'devops002', credentialsId: '84259fbb-0403-473e-9ae2-2d8105d57402', installation: 'ansible_server', playbook: '/var/lib/jenkins/workspace/Ansible-Tomcat_Deployment/package_deployment/', sudoUser: null
           echo "Deployment is successful!"
        }
     } 
  }
}
