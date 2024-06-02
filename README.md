Steps 
1. Launch EC2 and Connect it using SSH
2. Install Webserver into it
```
sudo yum update -y
sudo yum install git -y
git --version
git config --global user.name "username"
git config --global user.email "email-id"
sudo yum install httpd -y
sudo systemctl status httpd
sudo systemctl start httpd
 sudo systemctl status httpd
  sudo systemctl enable httpd
 sudo usermod -a -G apache ec2-user
sudo chmod 777 /var/www/html
pwd
cd /var/www/html
 pwd
ls
 sudo touch index.html
  sudo nano index.html
   ```
