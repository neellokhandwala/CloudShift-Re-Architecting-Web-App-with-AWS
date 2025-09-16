# Re-Architecting Web App on AWS Cloud [PaaS & SaaS]

## **Project Overview**
This project demonstrates the re-architecture of a sample web application on AWS Cloud using **PaaS and SaaS services**.  
It includes deployment of backend services, database setup, caching, message queue integration.

**AWS Services Used:**
- Amazon RDS (Relational Database Service)
- Amazon ElasticCache (Redis)
- Amazon ActiveMQ
- Elastic Beanstalk (Application Deployment)
- EC2 (for DB initialization)
- Elastic Load Balancer with HTTPS
- CloudFront CDN 

---

## **Deployment Workflow**
1. Login to AWS account.  
2. Create Key Pair for Beanstalk instance login.  
3. Create Security Groups for ElasticCache, RDS, and ActiveMQ.  
4. Launch AWS services:  
   - RDS Database  
   - ElasticCache  
   - ActiveMQ  
5. Create Elastic Beanstalk environment.  
6. Update Security Groups to allow traffic from Beanstalk.  
7. Launch EC2 instance to initialize RDS database.  
8. Update Beanstalk health check path to `/login`.  
9. Add HTTPS listener to Elastic Load Balancer (ELB).  
10. Build backend artifact and deploy to Elastic Beanstalk.  
11. Configure CloudFront CDN with SSL.  
12. Test the URL and verify deployment.

---
