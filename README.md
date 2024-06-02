Steps 

```
git clone
cd 
```

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
3. Create a bucket
4. Apply Bucket Policy

Tip:Note Down ARN of Bucket & paste it in policy
OR 
Generate Policy

and paste it
```
{
    "Version": "2012-10-17",
    "Statement": [
        {
            "Sid": "PublicReadGetObject",
            "Effect": "Allow",
            "Principal": "*",
            "Action": "s3:GetObject",
            "Resource": "arn:aws:s3:::your-bucket-name/*"
        }
    ]
}
```
6. Upload Coffee.img
7. Copy URL and paste in index.html
8. Check public ip of EC2 instance in web browser
