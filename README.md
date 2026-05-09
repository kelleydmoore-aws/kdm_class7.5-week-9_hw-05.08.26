# Class 7.5 Homework - Week 9 - 05.08.26

## Q & A:

### Load balancers:

1. &ensp; How does load balancing contribute to Fault tolerance? What about high availability?

2. &ensp; Do global load balancers decrease latency for end users? Why or why not?

3. &ensp; What are LB health checks for? Do we always need them? Is a LB different from a reverse proxy? 

4. &ensp; What are LB routing rules and URL maps for? Give an example or two of them in use. 

5. &ensp; Explain what an anycast IP address is used for in the context of a global load balancer. 

### Cloud Armor:

1. &ensp; What does cloud armor offer?
 
2. &ensp; Why is it used in the first place?

3. &ensp; What layer in the OSI model does it operate at? Why is this important and how is this firewall different from VPC firewall rules?
 
4. &ensp; What are rate based rules for?
 
5. &ensp; What is reCAPTCHA and how does it relate to this service? 

### Cloud CDN:

1. &ensp; What are POPs used for?

2. &ensp; What kind of files are served with Cloud CDN?
 
3. &ensp; What services can be used with cloud CDN for the source of content (the origin)?

4. &ensp; Does Cloud CDN help protect against any types of malicious actors or cyberattacks? Explain.

5. &ensp; Should an enterprise always use cloud CDN? Why or why not?

6. &ensp; What is TTL and how does it control content “freshness”?

## Runbook:

### Goal:

Create a Managed Instance Group (MIG) within the Google Cloud Platform (GCP) Console (ClickOps)

### Prerequisites:

1. &ensp; An active GCP project to build in.

2. &ensp; A Command Line Interface (CLI) configured to use GCP. It does not matter which one is used, only that it is correctly configured to create GCP projects in.

3. &ensp; GCP resources:

	a. &ensp; An Instance Template
	
	b. &ensp; Specific IAM permissions	

### Steps:

#### Creating Instance Template:

1. &ensp; In the search bar, navigate to Compute Engine.

2. &ensp; Within the left bumper in the Compute Engine screen, click on Instance Templates.

3. &ensp; Give the Instance Template a name in the Name field.

4. &ensp; Click within the Region dropdown field to select the region you wish to create the template in.

5. &ensp; In the Firewall section, select Allow HTTP traffic.

6. &ensp; Next, in the Advanced Options section, click on Networking.

7. &ensp; Ensure that in the Network tags section it has the http-server tag.

8. &ensp; Next click Network interface and ensure that default is selected in the dropdown.

9. &ensp; In the Management section, go to the Automation field and paste the contents of your metadata.sh script file into it.

10. &ensp; Once done with the previous steps, click Create to finish.

#### Creating the VM Instance:

1. &ensp; Within the left bumper in the Compute Engine screen, click on VM Instances then Create instance.

2. &ensp; In the Create an instance screen, at the top of the screen, click on Create VM from... then click Instance Template.

3. &ensp; Select the name of the Instance Template you just created in the previous step then click Create at the bottom of the screen.

4. &ensp; Wait until it is finished being built.

5. &ensp; Next, verify that it was created successfully by attempting to SSH into it.

6. &ensp; Under the connect tab of the new instance, click SSH. A new SSH browser window should launch. You may need to click Authorize to proceed with the connection.

7. &ensp; If it successfully connects through SSH, then the instance is up and running.

8. &ensp; Next, verify if the networking is set up correctly by pinging 8.8.8.8.

9. &ensp; If you get a response back, then the instance is functioning as intended.

10. &ensp; Next, verify that the external IP can be reached.

11. &ensp; Under the External IP tab, click on the IP address that is there.

12. &ensp; A new browser tab should launch and connect to a custom page based on the contents of your metadata.sh file.

13. &ensp; If this is successful, you now have a fully functioning VM instance created using and Instance Template.





