##### Dependencies

  - Terraform > 0.9
  - AWS keys exported as env variables
  - Packer > 1.1.2
  - Dynamic inventory setup
  - Python > 2.7
  - Ansible

# Put your Public key content here into the file file
- ./jenkins-master-setup-NEW/roles/jenkins_master/files/jenkins_id_rsa.pub
- ./jenkins-master-ami-NEW/roles/jenkins_master/files/jenkins_id_rsa.pub
- ./jenkins-slave-ami-NEW/roles/jenkins_slave/files/jenkins_id_rsa.pub
- ./my-ec2-jenkins-master-salve/ansible-code/jenkins-node/roles/jenkins_slave/files/jenkins_id_rsa.pub

# Put your Private key content here into the file file
- ./jenkins-master-setup-NEW/roles/jenkins_master/files/jenkins_id_rsa
- ./jenkins-master-ami-NEW/roles/jenkins_master/files/jenkins_id_rsa
- ./jenkins-slave-ami-NEW/roles/jenkins_slave/files/jenkins_id_rsa

  
