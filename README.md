# Streamlining Ticket Assignment for Efficient Support Operations

## 📌 Project Overview
This project implements an **automated ticket routing system** at **ABC Corporation** using **ServiceNow**, aimed at improving operational efficiency by assigning support tickets to the correct teams.

The solution reduces delays in issue resolution, enhances customer satisfaction, and optimizes resource utilization within the support department.

## 👨‍💻 Team Details
- **Team Leader:** Madhusudan  
- **Team Member 1:** Aaron  
- **Team Member 2:** Vignesh A S  
- **Team Member 3:** Abisheak C M  

## 🎯 Problem Statement
Manual ticket routing leads to:
- Delays in resolution  
- Misallocation of tickets  
- Inefficient use of support resources  

**Objective:** Automate ticket assignment using **ServiceNow workflows**, ensuring tickets are quickly routed to the correct team.

## 🛠️ Skills & Tools
- **Technologies:** TensorFlow, Spring  
- **Platform:** ServiceNow  

### Key Features
- User creation and management  
- Group and role assignments  
- Custom table creation for operations  
- Access Control Lists (ACL)  
- Automated Flow Designer for ticket routing  

## ⚙️ Implementation Steps

### 1. Create Users
- Navigate to **System Security → Users**  
- Add new users with required details  

### 2. Create Groups
- Navigate to **System Security → Groups**  
- Create groups for different support areas (e.g., Certificates, Platform)  

### 3. Create Roles
- Define roles under **System Security → Roles**  
- Assign roles to appropriate groups and users  

### 4. Create Tables
- Navigate to **System Definition → Tables**  
- Create a table named **Operations Related**  
- Define fields such as:  
  - *Issue* (Choices: Unable to login, 404 Error, Certificates, User Expired)  
  - *Assigned to Group*  

### 5. Assign Roles & Users to Groups
- Assign `Certification_role` to Certificates Group  
- Assign `Platform_role` to Platform Group  

### 6. Configure ACLs
- Create **Access Control Lists (ACLs)** to secure tables and fields  
- Ensure only authorized roles can access/update records  

### 7. Create Flows for Ticket Assignment
Using **ServiceNow Flow Designer**:
- **Flow 1:** Assign certificate-related issues → Certificates Group  
- **Flow 2:** Assign platform-related issues (login, 404 error, expired user) → Platform Group  

## ✅ Outcome
- Automated ticket assignment successfully implemented  
- Eliminated manual routing delays  
- Improved customer satisfaction with faster resolution times  
- Optimized support team workload distribution  

## 📊 Project Duration
Each module took approximately **1 hour** to configure and test.

## 📎 Additional Resources
For detailed step-by-step instructions and visuals, please refer to the included PDF document:  
`Streamlining_Ticket_Assignment_ABC_Corporation.pdf`

## 📌 Conclusion
By leveraging **ServiceNow’s automation capabilities**, this project demonstrates a **practical solution to streamline support operations**, making ticket management **faster, smarter, and more efficient**.
