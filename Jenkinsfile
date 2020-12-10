def workspace
pipeline 
{
  agent any
  stage('checkout') {
           steps {    
                git branch: 'master', url: 'https://github.com/egbea123/Ansible_Playbook.git'
          }
     }
     stage('Ansible Deploy')
     {    
        steps 
        { 
           sh "cd /var/lib/jenkins/workspace/Ansible-Tomcat_Deployment/package_deployment/Ansible_Playbook"
           sh  "ansible-playbook site.yaml"
           echo "Deployment is successful!"
        }
     }       
}
