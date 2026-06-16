# Incident-Management
Developed a Smart Incident Management System using Spring Boot, implementing RESTful APIs, layered architecture, and in-memory H2 database for efficient incident tracking and management.


# Smart Incident Management System

## 📌 Overview
This project is a Spring Boot-based Incident Management System designed to track and manage incidents efficiently. It allows users to create, view, and delete incidents while maintaining details such as status, priority, severity, and root cause analysis (RCA).

---

## 🚀 Features
- Create new incidents
- View all incidents
- Get incident by ID
- Delete incidents
- Track status (Open, In Progress, Resolved)
- Manage priority and severity
- Store RCA (Root Cause Analysis)

---

## 🏗️ Architecture
The application follows a layered architecture:

Client → Controller → Service → Repository → Database

---

## 🧰 Tech Stack
- Java 21
- Spring Boot
- Spring Data JPA
- H2 Database (for development)
- Maven
- Lombok

---

## 📂 Project Structure
com.akhilesh.incidentmanagement
├── controller
├── service
├── service.impl
├── repository
├── entity

---

## ⚙️ Setup

### 1. Run the Application
Run from IDE or:
```bash
mvn spring-boot:run

2. Access Application
http://localhost:8080

3. H2 Database Console
http://localhost:8080/h2-console


📡 API Endpoints
MethodEndpointDescriptionPOST/api/incidentsCreate IncidentGET/api/incidentsGet All IncidentsGET/api/incidents/{id}Get Incident by IDDELETE/api/incidents/{id}Delete Incident

🧪 Sample Request
JSON{  "title": "Server Down",  "description": "Production issue",  "status": "Open",  "priority": "High",  "severity": "Critical",  "rca": "Investigation ongoing"}``Show more lines

🎯 Learning Outcome

Built REST APIs using Spring Boot
Implemented layered architecture
Integrated database using JPA/Hibernate
Designed a real-world incident tracking system


✅ Future Enhancements

Update API
JWT Security
Search & filter
Docker & CI/CD

