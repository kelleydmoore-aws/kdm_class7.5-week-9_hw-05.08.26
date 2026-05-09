# Class 7.5 Homework - Week 9 - 05.08.26

## Q & A:

### Load balancers:

1. &ensp; How does load balancing contribute to Fault tolerance? What about high availability?

2. &ensp; Do global load balancers decrease latency for end users? Why or why not?

3. &ensp; What are LB health checks for? Do we always need them? Is a LB different from a reverse proxy? 

4. &ensp; What are LB routing rules and URL maps for? Give an example or two of them in use. 

5. &ensp; Explain what an anycast IP address is used for in the context of a global load balancer. 

	
### Cloud Armor:

1)	What does cloud armor offer?
 
2)	Why is it used in the first place?

3)	What layer in the OSI model does it operate at? Why is this important and how is this firewall different from VPC firewall rules?
 
4)	What are rate based rules for?
 
5)	What is reCAPTCHA and how does it relate to this service? 

### Cloud CDN:

1)	What are POPs used for?

2)	What kind of files are served with Cloud CDN?
 
3)	What services can be used with cloud CDN for the source of content (the origin)?

4)	Does Cloud CDN help protect against any types of malicious actors or cyberattacks? Explain.

5)	Should an enterprise always use cloud CDN? Why or why not?

6)	What is TTL and how does it control content “freshness”?


## Runbook:



### Goal:

Create a Managed Instance Group (MIG) within the Google Cloud Platform (GCP) Console (ClickOps)

### Prerequisites:

1)	An active GCP project to build in.

2)	A Command Line Interface (CLI) configured to use GCP. It does not matter which one is used, only that it is correctly configured to create GCP projects in.

3)	GCP resources:

	a)	An Instance Template
	
	b)	Specific IAM permissions
	

### Steps:

1)	In the search bar, navigate to Compute Engine.

