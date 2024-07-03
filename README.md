The project presented two challenges: improving website speed in the face of increased user traffic and strengthening security measures in response to an attempted ransomware security breach. The design choices that follow were carefully considered to address these issues and adhere to industry best practices.

We moved the MySQL database over to Amazon RDS to strengthen data protection. By taking this action, possible risks are mitigated, and industry compliance criteria are met by ensuring strong data encryption both in transit and at rest. Using RDS improves scalability and reliability while streamlining database administration.

Using Identity and Access Management, we put strict restrictions on administrative access in place. IAM roles were created, specifying exact rights and limiting access to just those who are permitted. Sensitive administration functions are protected by an extra security layer that is added by this specific access control layer.

We used Elastic Load Balancing in combination with Amazon CloudFront to provide safe and easy online user access. Through its material distribution Network, CloudFront not only expedites the distribution of material worldwide but also improves security by utilizing HTTPS encryption. In turn, ELB guarantees that incoming traffic is distributed evenly among several, thereby enhancing the website's responsiveness during traffic surges.

In accordance with economical and operational viability, a t2.micro EC2 instance was utilized for the deployment of the PHP application. This sort of instance satisfies the requirements and offers Secure Shell access for expedited administrative tasks. By using SSH, the EC2 instance gains an additional security layer that guarantees administrators have safe access.

Elastic Load Balancing was used to increase the website's availability. By dividing up incoming traffic among several EC2 instances, ELB produces a fault-tolerant design. By improving the website's overall resilience, this design choice ensures that users will always have a dependable and responsive experience even during periods of increased traffic.

We decided to use AWS Systems Manager Parameter Store to safely archive and handle database connection information since it prioritizes centralized configuration management and security. This complies with security best practices, guarantees that confidential data remains hidden in configuration files, and allows for easy changes.

With a preset launch template, AWS Auto Scaling was set up to adapt dynamically to changing workloads. Using an automated scaling method, the quantity of EC2 instances is changed in response to demand. Using a launch template speeds up scaling and provides uniformity and consistency when launching new instances, all while adhering to the project's requirement for autonomous scaling.

In conclusion, this all-encompassing strategy combines industry-leading security measures with the flexibility of AWS services, producing a solution ready to satisfy present demands as well as future scalability requirements. The combination of safe data processing, user-friendly interface design, and automated scalability sets up the Example Social Research Organization website for maximum efficiency and durability in the ever-changing field of international development statistics.
