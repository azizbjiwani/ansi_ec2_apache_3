Tutorial:
1. [creating an ec2 instance & adding keys to authorized_keys](http://www.bogotobogo.com/DevOps/Ansible/Ansible-aws-creating-ec2-instance.php)
2. [creating an ELB & registers an EC2 instance from the ELB](http://www.bogotobogo.com/DevOps/Ansible/Ansible-aws-creating-elb-and-register-ec2-instance.php)
# ansi_ec2_apache_3

ec2-user@ip-172-31-43-65 ansi_ec2_apache_3]$ pwd
/home/ec2-user/ansi_ec2_apache_3
[ec2-user@ip-172-31-43-65 ansi_ec2_apache_3]$ ansible-playbook site.yml

ec2-user@ip-172-31-43-65 ansi_ec2_apache_3]$ git init
Reinitialized existing Git repository in /home/ec2-user/ansi_ec2_apache_3/.git/
[ec2-user@ip-172-31-43-65 ansi_ec2_apache_3]$ git add -A
[ec2-user@ip-172-31-43-65 ansi_ec2_apache_3]$ git commit -m "ansible to create aws instance and update hosts"
[ec2-user@ip-172-31-43-65 ansi_ec2_apache_3]$ git remote add origin https://github.com/azizbjiwani/ansi_ec2_apache_3.git
[ec2-user@ip-172-31-43-65 ansi_ec2_apache_3]$ git push -u origin master

