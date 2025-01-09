pipeline{
  agent any
  stages{
      stage("Execute Playbook") {
          steps{
             ansiblePlaybook become: true, credentialsId: 'Ansible-PriKey-Ubuntu', installation: 'Ansible', inventory: '/etc/ansible/hosts', playbook: '/etc/ansible/playbook.yml', vaultTmpPath: ''
          }
      }

  }
}
