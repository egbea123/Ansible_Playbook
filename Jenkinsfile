def workspace
pipeline 
{
  agent any
    stages 
    {
      stage('checkout')
      {
           steps 
           {    
              git 'https://github.com/egbea123/Ansible_Playbook.git'            
              echo "Code successfully checked out!"
          }
     }
     stage('Ansible Deploy')
     {    
        steps 
        { 
           
           //sh " ansible-playbook /var/lib/jenkins/workspace/Ansible-Tomcat_Deployment/package_deployment/tomcatdeploy/site.yaml
           sh "cd /var/lib/jenkins/workspace/Ansible-Tomcat_Deployment/package_deployment/tomcatdeploy"
           sh  "ansible-playbook site.yaml"
           echo "Deployment is successful!"
        }
     }
    }    
        
}
