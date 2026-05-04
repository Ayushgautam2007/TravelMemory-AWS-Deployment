# TravelMemory MERN Stack Deployment on AWS

This project demonstrates the end-to-end deployment of a full-stack MERN (MongoDB, Express, React, Node.js) application on AWS, with a focus on scalability, load balancing, and production-level architecture.

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

## 🚀 Key Implementations
- Deployed a complete MERN stack application on AWS EC2 instances
- Configured Nginx as a reverse proxy and static file server
- Used PM2 for process management and ensuring backend availability
- Implemented horizontal scaling with multiple frontend and backend instances
- Set up Application Load Balancer with appropriate routing rules
- Integrated MongoDB Atlas for a managed database solution
- Enabled HTTPS and global content delivery using CloudFront

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

## 🎯 Objective
The primary goal of this project was to gain hands-on experience with deploying and managing a real-world full-stack application in a distributed AWS environment, including load balancing, scalability, and production best practices.
