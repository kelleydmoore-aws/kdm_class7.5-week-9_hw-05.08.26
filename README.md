# Class 7.5 Homework - Week 9 - 05.08.26

## Q & A:

### Load balancers:

-	How does load balancing contribute to Fault tolerance? What about high availability?

-	Do global load balancers decrease latency for end users? Why or why not?

-	What are LB health checks for? Do we always need them? Is a LB different from a reverse proxy? 

-	What are LB routing rules and URL maps for? Give an example or two of them in use. 

-	Explain what an anycast IP address is used for in the context of a global load balancer. 

	
### Cloud Armor:

-	What does cloud armor offer? 
-	Why is it used in the first place?
-	What layer in the OSI model does it operate at? Why is this important and how is this firewall different from VPC firewall rules? 
-	What are rate based rules for? 
-	What is reCAPTCHA and how does it relate to this service? 

### Cloud CDN:

-	What are POPs used for? 
-	What kind of files are served with Cloud CDN? 
-	What services can be used with cloud CDN for the source of content (the origin)? 
-	Does Cloud CDN help protect against any types of malicious actors or cyberattacks? Explain. 
-	Should an enterprise always use cloud CDN? Why or why not? 
-	What is TTL and how does it control content “freshness”?

## Runbook:



### Goal:

-	Create a Managed Instance Group (MIG) within the Google Cloud Platform (GCP) Console (ClickOps)

### Prerequisites:

-	An active GCP project to build in.
-	A Command Line Interface (CLI) configured to use GCP. It does not matter which one is used, only that it is correctly configured to create GCP projects in.
-	GCP resources:
	-	An Instance Template
	-	Specific IAM permissions

### Steps:

-	In the search bar, navigate to Compute Engine.

