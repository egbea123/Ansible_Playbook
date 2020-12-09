def workspace
pipeline 
{
  agent any
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
        
}
