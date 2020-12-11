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
          // ansiblePlaybook become: true, becomeUser: 'devops002', credentialsId: '84259fbb-0403-473e-9ae2-2d8105d57402', installation: '192.168.0.29', playbook: '/var/lib/jenkins/workspace/Ansible-Tomcat_Deployment/package_deployment/site.yaml', sudoUser: null
           ansiblePlaybook credentialsId: 'MIIEpAIBAAKCAQEAxVPfPi/5WhtTx3Oc42IGU7mz82yhD+MxlShVXI4PYi7vGu9a
ObSOfS6kRgjzz9RtXRsW3uXk6SvsFDom8XXJ/ETH5JYOE2C8JKWADCOa8muCtHZO
+wtOPnE4C4wzOMZFa4cz4Sg3Hweeo4XAkCCBsoijCs3cZzoxvZI1kC8Trmptx++W
Dkl9xg/C4qy8Z4euPjmGMfRu+gfizXap2HI/ARTV0ulOKlYT40mNA2YYtT8fYGkq
waZwf0MTNnJactcJ5ZEFK1aapZSxj5KPxyqQPTeTfUur0mRK1F8yx/MO06UhyR2Y
v7d6+ktXNY5C1yTT+UPFq6ks8/c/7f3d/AqrowIDAQABAoIBAQC+/hxBK9wU3Ahu
L7f12iY3mbHUdhs6rnOKZHyi1hmLtdPW5T8WRW35OlDkPLwIOBsWmCa93hR/n/Sj
61lQMusrEkPMO3UqSmIwskPK/Bd4dpkPJMfzcxDrnVhazPuzAy2kEzwivXMExLJG
oiotFlmSvW/aAEFJZOlKDJ9tjDNnh4bcou1Z+6PGTYCNJ8czJQdfLlyaDE5x+te4
OB9m8QjBT0532uB06RRMH1FSNaM27bJp1/VZZZEtLgacxyDVJmtfmYrUz8oWZlbH
ecxho8z0UmjAiXPcdySzU5XLeMOR4j8ZozXHD+qSrunG8rwPz40gBYKTYjQVFyZa
DslhQwqRAoGBAOGkwk4lb/ZgkMS4RJAkS52/91n6rM3mGu+9F7GWZopTZBDA1OMn
pFGjaQTdXv9bRuT7UCky8PCVLWZbJAF1c+iSo63mbbKY9Ltztp6e5BHm2pn+aqfX
', inventory: 'webserver', playbook: 'site.yaml'
        }
     } 
  }
}
