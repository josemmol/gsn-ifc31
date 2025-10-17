1. Review the practice lab tasks in the Concept section.
1. Click Start Lab or Open AWS Console to begin.
1. Follow the lab instructions carefully, and use the arrows to navigate between steps.
### dsaffdf

1. In the top navigation bar search box, type:
ec2
1. In the search results, under Services, click EC2.
1. Go to the next step.

1. On the Dashboard, click Launch instance.
2. Go to the next step.

1. In the Name and tags section, for Name, type a name that you like, such as webserver01.
2. In the Application and OS Images section, under Quick Start, choose Amazon Linux.
3. Go to the next step.

1. For Amazon Machine Image (AMI), on the dropdown list, keep or choose Amazon Linux 2023 AMI.
2. For Instance type, click Compare instance types.
3. Go to the next step.

1. In the Instance types section, review the available instances and their associated resources.
2. Choose the t3.micro instance type.
3. Click Get advice.
4. Go to the next step.

1. To see instance type and family recommendations for various workloads, in the pop-up box, review the different instance type requirements.

- You can use the dropdown lists to experiment with different requirements, clicking Get instance type advice for each new requirement.

2. When finished, close the pop-up box.
3. At the bottom of the page, click Select instance type.
4. Go to the next step.

1. Review to confirm that the t3.micro instance type is selected.
2. For Key pair name, choose Proceed without a key pair. 
3. In the Network settings section, click Edit.
4. Go to the next step.

1. For VPC, choose cloud-first-steps/LabVpc.

- Your solution will fail if you do not choose this VPC.

2. For Subnet, choose the subnet in the us-east-1a Availability Zone.

- Note the AZ choices on the dropdown list. In the upcoming DIY section of this solution, you must choose the subnet in the other AZ.

3. Go to the next step.

1. For Security group name, type: 

Lab-SG

2. For Description, type: 

HTTP Security Group

3. For Type, choose HTTP.
4. In the warning alert, review the message.

- Port 80 (HTTP) is accessible from the internet. While web servers need public access, security group rules should be as restrictive as possible.

5. Go to the next step.

1. In the Configure storage section, keep the default selection of an 8 GiB gp3 volume. 
2. Click to expand Advanced details.
3. Go to the next step.

1. For User data, click Choose file.
2. In the pop-up box (not shown), choose the user-data.txt file that you downloaded to your device in an earlier step, and then review the file contents.
3. Go to the next step.

1. Review the Summary section.  

- When your browser is fully expanded, this section floats on the right side. 

2. Click Launch instance.
3. Go to the next step.

1. In the success alert, review the message.
2. Go to the next step.

1. At the bottom of the page, click View all instances.
2. Go to the next step.

1. In the Instances section, choose the checkbox to select the available EC2 instance.
2. Wait 2–3 minutes, and then click the section's refresh icon.
3. Under Instance state, review to confirm that the instance is now running.

- The change from Pending to Running might take several minutes, and you might need to refresh several times.

4. For the running instance, on the Details tab, under Public IPv4 DNS, click the copy icon to copy the provided address.

- Do not click the "open address" link.

5. Go to the next step.

1. In a new browser tab (or window) address bar, type:

http://

2. Next to http://, paste the DNS address that you just copied and press Enter.
3. On the page, review the details about your instance.

- If you see a connection timeout message when opening the webpage, check that the address begins with http:// and not https://.
- The public DNS and the security group are used to access the instance details that appear on the webpage. The public DNS record translates a domain name to an IP address. The record informs the browser which server to connect to.

4. Go to the next step.

Congratulations! You've completed the Practice section. Go to the DIY section to complete the solution.
