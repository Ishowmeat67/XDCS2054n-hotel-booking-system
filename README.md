
XDCS2054N Introduction to Cloud Computing - Hotel Booking Management System (CloudEats Domain Migration)
Hotel Booking Management System (Microservices)

Course: XDCS2054N Introduction to Cloud Computing  
Semester: September 2026  
Assignment: CloudEats Domain Migration  

---

 1. Project Overview
This project adapts the original 3-microservice CloudEats application into an enterprise **Hotel Booking Management System**. All original food and menu references have been migrated to hotel operations, featuring room inventory management, reservation tracking, and guest profiles.

 Architecture Overview
The system consists of three independent microservices, each backed by its own dedicated database and connected over an isolated Docker bridge network:

Guest Service (`guest-service`): Manages guest accounts, identity records, and profile details.
Room Service (`room-service`): Handles room catalog listings, room categories (Deluxe, Suite, Standard), per-night pricing, and room status.
Booking Service (`booking-service`): Orchestrates reservations, stay date calculations, status updates, and booking receipts.

---

 2. Prerequisites
Ensure you have the following installed on your host machine or VM:
Docker Engine (v24.0+ recommended)
Docker Compose (v2.20+ recommended)
Git
cURL or Postman (for API testing)

---

 3. Environment Configuration
Environment variables are managed using a `.env` file in the root directory.

1. Copy the sample environment file:
   ```bash
   cp .env.example .env
