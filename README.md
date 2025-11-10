# 💰 One India Pay
## Microservices Fintech Platform

[![Java](https://img.shields.io/badge/Java-17-orange.svg)](https://www.oracle.com/java/)
[![Spring Boot](https://img.shields.io/badge/Spring%20Boot-3.x-brightgreen.svg)](https://spring.io/projects/spring-boot)
[![PostgreSQL](https://img.shields.io/badge/PostgreSQL-12+-blue.svg)](https://www.postgresql.org/)
[![License](https://img.shields.io/badge/License-Proprietary-red.svg)](LICENSE)
[![Build Status](https://img.shields.io/badge/Build-Passing-brightgreen.svg)](https://github.com/yourusername/one-india-pay)

> A comprehensive fintech platform built with Spring Boot microservices architecture

## 🚀 Overview

One India Pay is a **modern fintech platform** designed for seamless payment processing, user management, and commission distribution. Built with **microservices architecture** for scalability and maintainability.

## ✨ Features

### 👥 User Management
- 🔐 **JWT Authentication**
- 🏢 **Role-based Hierarchy** 
- 📊 **Status Management**
- 🔒 **Data Encryption**

### 💳 Payment Processing
- 💰 **Razorpay Integration**
- 🔄 **Real-time Processing**
- 📈 **Transaction Tracking**
- 🛡️ **Secure Payments**

### 👛 Digital Wallet
- 💵 **Balance Management**
- 🔐 **Encrypted Storage**
- ⚡ **Instant Transfers**
- 📱 **Mobile Ready**

### 💼 Commission System
- 📊 **Hierarchical Distribution**
- ⚙️ **Configurable Rates**
- 🤖 **Auto Setup**
- 👨💼 **Admin Controls**

## 🏗️ Architecture


Client Applications
↓
API Gateway
↓
Service Registry
↓ ↓ ↓
User Service → User DB
Wallet Service → Wallet DB
Commission Service → Commission DB
Payment Service → Razorpay API
Auth Service
Transaction Service
Admin Service



## 🔧 Technology Stack

| Category | Technology |
|----------|------------|
| **Backend** | Java 17, Spring Boot 3.x |
| **Database** | PostgreSQL 12+ |
| **Security** | JWT, BCrypt Encryption |
| **Payment** | Razorpay Integration |
| **Build** | Maven 3.6+ |
| **Discovery** | Netflix Eureka |

## 🎯 Services Overview

| Service | Port | Status | Description |
|---------|------|--------|-------------|
| 🌐 **Service Registry** | 8761 | ✅ Complete | Netflix Eureka for service discovery |
| 👤 **User Service** | 8081 | ✅ Complete | User management & authentication |
| 💰 **Wallet Service** | 8082 | ✅ Complete | Digital wallet operations |
| 💼 **Commission Service** | 8083 | ✅ Complete | Commission calculation & distribution |
| 💳 **Payment Service** | 8084 | ✅ Complete | Razorpay payment processing |
| 📊 **Transaction Service** | 8085 | 🔄 In Progress | Transaction management |
| 🔐 **Auth Service** | 8086 | 🔄 In Progress | Centralized authentication |
| ⚙️ **Admin Service** | 8087 | 🔄 In Progress | Administrative dashboard |

## 🚀 Quick Start

### 📋 Prerequisites
- ☑️ Java 17+
- ☑️ PostgreSQL 12+
- ☑️ Maven 3.6+
- ☑️ Razorpay Account

### ⚡ Installation

1. **Clone the repository**
```bash
git clone https://github.com/yourusername/one-india-pay.git
cd one-india-pay

📚 API Documentation
👤 User Service APIs
Method	Endpoint	Description
POST	/users/register	Register new user
GET	/users/{id}	Get user details
GET	/users/hierarchy/{parentId}	Get user hierarchy
PUT	/users/{id}	Update user
DELETE	/users/{id}	Deactivate user
💰 Wallet Service APIs
Method	Endpoint	Description
POST	/wallets/create/{userId}	Create wallet
GET	/wallets/{userId}	Get wallet details
POST	/wallets/credit	Credit wallet
POST	/wallets/debit	Debit wallet
💼 Commission Service APIs
Method	Endpoint	Description
POST	/commissions	Set commission
GET	/commissions/{userId}	Get commission details
POST	/commissions/calculate	Calculate commission
PUT	/commissions/admin	Update admin commission
💳 Payment Service APIs
Method	Endpoint	Description
POST	/payments/create-order	Create payment order
GET	/payments/order/{orderId}	Get order details
🔒 Security Features
🔐 JWT Authentication - Secure token-based auth

🔒 BCrypt Encryption - Password hashing

🛡️ Role-based Access - Hierarchical permissions

🔍 Input Validation - Comprehensive sanitization

🚫 SQL Injection Prevention - Parameterized queries

📊 Audit Logging - Complete activity tracking

📊 Development Progress
Component	Progress
Core Services	100% ✅
Database Design	100% ✅
API Implementation	85% 🔄
Security	90% 🔄
Testing	60% 🔄
🗺️ Roadmap
 🔐 Complete Authentication Service
 📊 Transaction Service implementation
 ⚙️ Admin Dashboard
 🧪 Comprehensive testing
 📖 Swagger documentation
 📈 Monitoring & logging
 ⚡ Performance optimization
 🚀 CI/CD pipeline
🏢 Business Logic
User Hierarchy
Admin → Can add Super Distributors, Distributors, Retailers

Super Distributor → Can add Distributors and Retailers

Distributor → Can add Retailers only

Retailer → Cannot add users

Commission Flow
Transaction occurs

Commission calculated based on hierarchy

Admin gets admin commission rate

Parent gets parent commission rate

Remaining amount goes to user

Wallet Operations
Secure balance encryption

Real-time balance updates

Transaction history tracking

Insufficient balance validation

🤝 Contributing
🍴 Fork the repository

🌿 Create feature branch (git checkout -b feature/AmazingFeature)

💾 Commit changes (git commit -m 'Add AmazingFeature')

📤 Push to branch (git push origin feature/AmazingFeature)

🔄 Open Pull Request

📄 License
This project is proprietary software. All rights reserved.
