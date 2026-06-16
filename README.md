Employee Management System

A production-ready Full-Stack Employee Management interface built to optimize administrative workflows, department monitoring, and leave request cycles. 

 Live Interactive Demo
* **Live Sandbox URL:** [https://employee-ms-nine.vercel.app/start]
* *Note: The live link features an adaptive demo sandbox fallback configuration that automatically intercepts API requests and loads fluid, interactive local mockup states when isolated from the production MySQL container database.*

---
 Technology Stack
* **Frontend:** React.js, Axios, HTML5/CSS3, Bootstrap, Vite
* **Backend Platform:** Node.js, Express.js
* **Database Management:** MySQL, phpMyAdmin

---
 Architectural Features & Highlights
* **Centralized Network layer:** Leverages a custom, reusable Axios client network instantiation layer to streamline base server environment toggling securely.
* **UI Resiliency Fallbacks:** Uses advanced optional chaining mechanisms and conditional logical operators to ensure graceful loading state fallbacks and eliminate blank-screen layout rendering failures.
* **Interactive Control Pipelines:** Implements granular administrative permission structures, enabling seamless dashboard state metric updates on employee leave processing events.

---
 Local Environment Quick Start

To spin up the comprehensive project architecture locally with full database integration on your machine, follow these execution steps:

 1. Database Schema Setup
Initialize your MySQL system server instance and execute the following structural setup schema scripts:

```sql
CREATE DATABASE IF NOT EXISTS employeems;
USE employeems;

CREATE TABLE IF NOT EXISTS category (
    id INT AUTO_INCREMENT PRIMARY KEY,
    name VARCHAR(255) NOT NULL
);

CREATE TABLE IF NOT EXISTS employee (
    id INT AUTO_INCREMENT PRIMARY KEY,
    name VARCHAR(255) NOT NULL,
    email VARCHAR(255) UNIQUE NOT NULL,
    salary INT NOT NULL,
    address VARCHAR(255) NOT NULL,
    category VARCHAR(255) NOT NULL
);
```
 2. Backend Server Application Build
Navigate to your server directory terminal and execute:
```bash
npm install
npm run start
```
 3. Client Interface Initialization
Navigate into the core frontend directory terminal profile and run:
```bash
npm install
npm run dev
```
