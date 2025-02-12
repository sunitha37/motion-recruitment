aws

Visit the AWS Website:

Go to the official AWS website at aws.amazon.com.
Start the Sign-Up Process:

Click on the "Create an AWS Account" button.
Provide Personal Information:

Enter your email address, password, and AWS account name.
Verify Email Address:

Check your email for a verification message from AWS and follow the provided link to verify your email address.
Add Contact Information:

Fill in your personal or professional contact details as required.
Choose Account Type:

Select the account type (e.g., personal or business).
Payment Information:

Enter credit card information for billing purposes. Note that AWS offers a free tier for new accounts.
Identity Verification:

Complete the verification process, which may involve receiving a code via SMS or a phone call.
Select Support Plan:

Choose the basic support plan if you are just starting out, which is free of cost.
Completion:

Once all steps are verified and completed, you will receive a confirmation email indicating that your AWS account is active.
Step 2: Setting Up a Basic EC2 Instance
Log In to the AWS Management Console:

Use your credentials to log in at aws.amazon.com.
Navigate to EC2 Dashboard:

From the Console home, navigate to the “EC2” service under the “Compute” section.
Launch Instance:

Click the “Launch Instance” button to start configuring your new instance.
Choose AMI (Amazon Machine Image):

Select an Amazon Machine Image (AMI). For this example, choose the “Amazon Linux 2 AMI” which is free tier eligible.
Choose Instance Type:

Select an instance type. For basic tasks, the "t2.micro" instance is sufficient and free tier eligible.
Configure Instance:

Proceed with the default configurations. You can configure network settings if needed, but default settings should work for a basic setup.
Add Storage:

Specify storage size. The default 8 GB is usually sufficient for basic tasks.
Add Tags:

Add tags for easier management (e.g., Key: Name, Value: MyFirstInstance).
Configure Security Group:

Set up a security group to define firewall rules. Allow SSH access by adding a rule to allow incoming traffic on port 22 from your IP address.
Add a rule to allow HTTP traffic on port 80 to access your deployed Python script.
Review and Launch:

Review your settings and click “Launch”.
Key Pair:

You will be prompted to create a new key pair or use an existing one. Download and save the key pair securely as you will need it to access the instance.
Launch Instance:

Click "Launch Instances". You should see confirmation that your instance is launching.
Step 3: Deploying a Sample Python Script
Connect to Your EC2 Instance:

Navigate to the “Instances” section in the EC2 Dashboard.
Select your instance and click on the “Connect” button.
Follow the on-screen instructions to connect to your instance using SSH. Use a command like ssh -i "your-key-pair.pem" ec2-user@your-ec2-instance-public-dns.
Install Python:

Update the package index and install Python if it’s not already installed. You can usually do this using commands like sudo yum update and sudo yum install python3.
Create a Python Script:

Use a text editor (e.g., nano, vi) to create a Python script. For example, you can create a file named add_numbers.py using a command like nano add_numbers.py.
Write the Python Code:

Open the add_numbers.py file and write the script that adds two numbers.
Test the Script:

Run the script using the Python interpreter to ensure it works as expected. Use a command like python3 add_numbers.py.
Ensure Script Accessibility:





