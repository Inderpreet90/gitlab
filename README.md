# GitLabEC2

## Create Ec2 instance and install GitLab Community Edition on it

### At the end you will be able to access your GitLab server using your ec2 public URL

##### For Example: 
http://ec2-xx-xx-xx-xx.compute-1.amazonaws.com

### Use below given Ansible Ad-Hoc command to run the playbook
ansible-playbook -i inventory/gitlabec2/ playbooks/gitlab.yaml

## Notes (gitlabonec2)
 - Remember to place your self signed ssl certificate (.pem file) in files directory under gitlabec2 role
 - Remember to replace the file name in gitlab_install.yml playbook accordingly



# GitLabHA (In-Progress)

## Configure High Availability environment using AWS autoscaling for GitLab

### Use below given Ansible Ad-Hoc command to run the playbook
ansible-playbook -i inventory/gitlabha playbooks/gitlab-network.yaml

## Notes (gitlabHA)
 - I have tested this on latest version of Ansible and Boto3 hence recommend the same 
