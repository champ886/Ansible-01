pipeline{
  agent any
  stages{
      stage("Execute Playbook") {
          steps{
              ansiblePlaybook become: true, credentialsId: 'Ansible-Ubuntu', installation: 'Ansible', inventory: '/etc/ansible/hosts', playbook: '/home/champ/playbook.yml', vaultTmpPath: ''
          }
      }

  }
}
