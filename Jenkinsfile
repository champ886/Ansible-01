pipeline{
  agent any
  stages{
      stage("Execute Playbook") {
          steps{
            sh 'ansible-playbook /home/champ/playbook.yml -i /etc/ansible/hosts'
             ansiblePlaybook become: true, credentialsId: 'Ansible-Centos-Direct', installation: 'Ansible', inventory: '/etc/ansible/hosts', playbook: '/home/champ/playbook.yml', vaultTmpPath: ''
          }
      }

  }
}
