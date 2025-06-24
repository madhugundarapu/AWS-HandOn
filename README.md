# AWS-HandOn
practical experience 
# Internshala Practice
# how to login SSH and launch ec2 instance
$ ssh ec2-user@public ip
The authenticity of host '43.205.243.101 (43.205.243.101)' can't be established.
ED25519 key fingerprint is SHA256:4Vo5Pr9OTdKVyxfGN9aPk1S/vRUXN0f6CcWsDLuu0DQ.
This key is not known by any other names.
Are you sure you want to continue connecting (yes/no/[fingerprint])? yes
Warning: Permanently added '43.205.243.101' (ED25519) to the list of known hosts.
ec2-user@43.205.243.101: Permission denied (publickey,gssapi-keyex,gssapi-with-mic).

C:\Users\madhu>cp Downloads
'cp' is not recognized as an internal or external command,
operable program or batch file.

C:\Users\madhu>cd Downloads

C:\Users\madhu\Downloads>ls -s packup.pem
'ls' is not recognized as an internal or external command,
operable program or batch file.
$ssh -i packup.pem ec2-user@public ip
# WARNING: UNPROTECTED PRIVATE KEY FILE
Permissions 0644 for packup.pem are TOO OPEN
# PERMISSION DENIED 
$chmod 0400 packup.pem
$ssh -i packup.pem ec2-user@public ip
logined EC2 Instance
# install httpd  
$ sudo yum update 
this command will update 
$ sudo yum install httpd -y
it will install http
$ sudo systemctl start httpd
it will start service but not shown output
$ sudo systemctl status httpd
it will shown output like
# active in green color
goto ec2 instance copy public ip and paste it on the web it will shown httpd web page


