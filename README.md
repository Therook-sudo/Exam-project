# Landing Page Deployment

## Project Overview
This repository contains the documentation and setup files for deploying a Linux server and hosting a simple HTML landing page. 

### Features
- Provisioned an AWS EC2 instance with Ubuntu.
- Installed Apache as the web server.
- Deployed a custom HTML page containing my bio, project title, and description.
- Configured networking for HTTP access.
- installed dependencies using sudo apt install software-properties-common
- installed cerbot ( sudo apt install certbot python3-certbot-apache)
- connected domain name to instance ip 
- ran certbot to obtain and install SSL certificate (sudo certbot --apache )
- deployed SSL certificate using let's encrypt
 
## Public IP Address
[https://emekatherook.com.ng/](https://emekatherook.com.ng/)
<3.86.160.161>

## Steps to Recreate
1. **Provision the Server**
   - Launched an AWS EC2 instance using Ubuntu 20.04 LTS.
   - Allowed HTTP and SSH traffic in the security group.

2. **Install Apache**
   - Updated package lists and installed Apache.
   - Verified the server by accessing `public-ip'.
 

3. **Deploy HTML**
   - Created a custom `index.html` in `/var/www/html`.
   - Updated permissions for the file.

4. **Configure Networking**
   - Opened port 80 for HTTP traffic in the AWS security group.
   - opened port 22 to enable ssh into the server 
   - opened port 443 for HTTPS traffic into the DNS of the instance 

## Screenshot
![Landing Page Screenshot](screenshot.png)

##  HTTPS Configuration
- Installed Certbot for SSL certificates.
- Configured Apache to serve content over HTTPS.

### Repository Content
- `index.html`: The deployed HTML file.
- `README.md`: Documentation for setup and deployment.
- `screenshot.png`: screenshot of the html page
---


