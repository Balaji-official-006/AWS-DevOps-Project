Launch an EC2 Instance:

Go to the AWS Management Console.

Navigate to the EC2 dashboard and click "Launch Instance."

Choose an Amazon Linux 2 or Ubuntu AMI (Amazon Machine Image).

Select an instance type (like t2.micro for a free tier).

Configure instance details, add storage, and configure security group.

For the security group, allow HTTP (port 80) and SSH (port 22) access.

Review and launch the instance, and download the key pair if you haven’t already.

Connect to Your EC2 Instance:

Use SSH to connect to your instance. For example:

ssh -i /path/to/your-key.pem ec2-user@your-ec2-public-dns


Update the Package Repository:

Once connected, update the package lists:

sudo yum update -y    # For Amazon Linux
sudo apt update -y     # For Ubuntu


Install HTTPD (Apache):

For Amazon Linux:

sudo yum install httpd -y


For Ubuntu:

sudo apt install apache2 -y


Start and Enable the Apache Service:

On Amazon Linux:

sudo systemctl start httpd
sudo systemctl enable httpd


On Ubuntu:

sudo systemctl start apache2
sudo systemctl enable apache2


Configure the Firewall (if needed):

Ensure your security group allows inbound traffic on port 80.

Verify the Installation:

Open a browser and go to your EC2 instance's public DNS or IP address. You should see the Apache test page.
