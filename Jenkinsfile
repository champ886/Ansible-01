pipeline{
  agent any
  stages{
      stage("Execute Playbook") {
          steps{
              ansiblePlaybook credentialsId: 'Ansible-PriKey-Ubuntu', installation: 'Ansible', inventory: '/etc/ansible/hosts', playbook: '/home/champ/playbook.yml', vaultTmpPath: ''
          }
      }

  }
}
