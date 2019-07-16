Tutorial:
1. [creating an ec2 instance & adding keys to authorized_keys](http://www.bogotobogo.com/DevOps/Ansible/Ansible-aws-creating-ec2-instance.php)
2. [creating an ELB & registers an EC2 instance from the ELB](http://www.bogotobogo.com/DevOps/Ansible/Ansible-aws-creating-elb-and-register-ec2-instance.php)
# ansi_ec2_apache_3

ec2-user@ip-172-31-43-65 ansi_ec2_apache_3]$ pwd
/home/ec2-user/ansi_ec2_apache_3/CreatingEC2    
[ec2-user@ip-172-31-43-65 CreatingEC2]$ ansible-playbook site.yml  
ec2-user@ip-172-31-43-65 ansi_ec2_apache_3]$ vi hosts  
[local]  
localhost  
[webserver]  
3.94.120.76 ansible_ssh_user=ubuntu ansible_ssh_private_key_file=../aws-private.pem  
  
ec2-user@ip-172-31-43-65 ansi_ec2_apache_3]$ git init  
Reinitialized existing Git repository in /home/ec2-user/ansi_ec2_apache_3/.git/  
[ec2-user@ip-172-31-43-65 ansi_ec2_apache_3]$ git add -A  
[ec2-user@ip-172-31-43-65 ansi_ec2_apache_3]$ git commit -m "ansible to create aws instance and update hosts"  
[ec2-user@ip-172-31-43-65 ansi_ec2_apache_3]$ git remote add origin https://github.com/azizbjiwani/ansi_ec2_apache_3.git  
[ec2-user@ip-172-31-43-65 ansi_ec2_apache_3]$ git push -u origin master  

  
update site.yml with public ip of newly created remote host   
AddingKeys/site.yml      
  hosts: 3.81.149.60   
  
Always delete aws-private.pem key file under project directory (ansi_ec2_apache_3) while creating the new project (or during first run of the project)  




