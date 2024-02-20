AWS Lift and Shift: Application Workload Migration
Project Overview
Welcome to the AWS Lift and Shift project! In this cloud computing initiative, we aim to migrate a multi-tier web application stack named "vprofile" from a local setup using Vagrant to a production environment on AWS. The migration strategy we'll employ is the "lift and shift" approach.

Project Objectives
Flexible Infrastructure: Transition from a local data center to AWS for a more flexible and scalable infrastructure.

Pay-as-You-Go Model: Embrace the AWS cloud computing model, allowing us to pay for resources as we use them.

Modernization: Enhance the application's efficiency by utilizing AWS services for improved performance.

Automation: Implement infrastructure as code for seamless management, scalability, and cost control.

Project Scenario
Our current scenario involves a variety of application services running on physical or virtual machines within a local data center. This setup requires multiple teams for virtualization, data center operations, monitoring, and system administration, leading to complexity, high costs, and manual processes.

AWS Services Utilized
EC2 Instances: Virtual machines for services like Tomcat, RabbitMQ, Memcache, and MySQL.

Elastic Load Balancer: Replacing the engine service for load balancing.

Auto Scaling: Automatically scaling EC2 instances based on demand, optimizing resource usage and cost.

Storage: Utilizing S3 or EFS for storage needs.

Additional Services: IAM, ACM, EBS, Route 53 for private DNS, and more.

Architectural Design
Before AWS Migration

After AWS Migration

Execution Flow
AWS Account Setup:

Log into your AWS account and configure key pairs for EC2 instance access.
Security Group Creation:

Create security groups for the load balancer, Tomcat instances, and backend services.
Launch Instances:

Launch EC2 instances with user data scripts, setting up essential configurations.
Route 53 Configuration:

Update IP-to-name mappings in Route 53 for DNS resolution.
Build and Upload Artifacts:

Build the application from source code locally, then upload the artifacts to an S3 bucket.
Load Balancer Setup:

Configure the elastic load balancer with HTTPS connection.
DNS Mapping:

Map the elastic load balancer endpoint to a website in GoDaddy DNS.
Auto Scaling Group:

Implement an auto-scaling group for Tomcat instances, ensuring scalability based on demand.
Verification:

Verify the entire setup, ensuring proper functionality and performance.

Conclusion
The AWS Lift and Shift project demonstrates the power of cloud computing in migrating and optimizing application workloads. By leveraging AWS services, we achieve flexibility, scalability, and automation, ultimately enhancing the overall efficiency of our application.

Feel free to explore, contribute, and join us on this cloud journey!

Happy coding!