## Create Ec2 instance and install GitLab Community Edition on it

### At the end you will be able to access your GitLab server using your ec2 public URL

##### For Example: 
http://ec2-xx-xx-xx-xx.compute-1.amazonaws.com

### Use below given Ansible Ad-Hoc command to run the playbook
ansible-playbook -i inventory/ playbooks/gitlab.yaml

## Notes
 - Remember to place your self signed ssl certificate (.pem file) in files directory under gitlabec2 role
 - Remember to replace the file name in gitlab_install.yml playbook accordingly
