pipeline{
  agent any
  stages{
      stage("Execute Playbook") {
          steps{
             ansiblePlaybook become: true, installation: 'Ansible', inventory: '/etc/ansible/hosts', playbook: '/etc/ansible/playbook.yml', vaultTmpPath: ''
          }
      }

  }
}
