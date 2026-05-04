# TravelMemory MERN Stack Deployment on AWS

This project demonstrates the end-to-end deployment of a full-stack MERN (MongoDB, Express, React, Node.js) application on AWS, with a focus on scalability, load balancing, and production-level architecture.

---

## 🔗 Live Application
https://d6bisv02umd0e.cloudfront.net/

---

## 🏗️ Architecture Overview
**User → CloudFront → Application Load Balancer → EC2 Instances → MongoDB Atlas**

### Components
- **Frontend:** React application served via Nginx (2 EC2 instances)
- **Backend:** Node.js API managed with PM2 (2 EC2 instances)
- **Database:** MongoDB Atlas (cloud-hosted)
- **Load Balancing:** AWS Application Load Balancer (ALB)
- **Content Delivery & HTTPS:** AWS CloudFront

---

## 🖼️ Architecture Diagram
<img width="940" height="644" alt="image" src="https://github.com/user-attachments/assets/74013530-89c1-4041-90fe-e83a4e9141c1" />

---

## 🚀 Key Implementations
- Deployed a complete MERN stack application on AWS EC2 instances
- Configured Nginx as a reverse proxy and static file server
- Used PM2 for process management and ensuring backend availability
- Implemented horizontal scaling with multiple frontend and backend instances
- Set up Application Load Balancer with routing rules
- Integrated MongoDB Atlas for a managed database solution
- Enabled HTTPS and global content delivery using CloudFront

---

## ⚙️ Deployment Steps
1. Launched EC2 instances for frontend and backend  
2. Installed Node.js, Nginx, and PM2  
3. Deployed backend and started using PM2  
4. Built frontend and served via Nginx  
5. Configured reverse proxy in Nginx  
6. Set up Application Load Balancer  
7. Connected MongoDB Atlas  
8. Configured CloudFront for HTTPS  

---

## 📌 Tech Stack

- Frontend: React
- Backend: Node.js, Express
- Web Server: Nginx
- Process Manager: PM2
- Cloud: AWS (EC2, ALB, CloudFront)
- Database: MongoDB Atlas


---

## ⚠️ Challenges Encountered
- Mixed content issues due to HTTP/HTTPS mismatch  
- CORS configuration errors between frontend and backend  
- Blank screen issues caused by incorrect frontend build deployment  
- CloudFront caching inconsistencies  

---

## 🛠️ Resolutions
- Replaced hardcoded backend URLs with relative `/api` endpoints  
- Rebuilt and redeployed the frontend correctly across all instances  
- Corrected Nginx configuration for static content and routing  
- Tuned CloudFront caching behavior and invalidations  

---

## 🧪 Health Checks
- ALB health checks configured for backend APIs  
- Verified application availability across multiple instances  

---

## 🛡️ Security Considerations
- Secured APIs behind Application Load Balancer  
- Enabled HTTPS via CloudFront  
- Used environment variables for sensitive data  
- Configured Security Groups to restrict access  

---

## 📈 Future Improvements
- Implement Auto Scaling Groups for EC2  
- Add CI/CD pipeline (GitHub Actions / Jenkins)  
- Containerize application using Docker  
- Use Terraform for Infrastructure as Code  
- Add monitoring with CloudWatch and Prometheus  

---

## 🧠 Key Learnings
- Real-world deployment challenges in distributed systems  
- Handling CORS and HTTPS issues in production  
- Load balancing and multi-instance architecture  
- Understanding CDN caching behavior  

---

## 🎯 Objective
The primary goal of this project was to gain hands-on experience with deploying and managing a real-world full-stack
