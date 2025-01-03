# Postman-xlr8

# 🌟 Postman API Testing Project

## 📖 Overview
This project demonstrates an end-to-end implementation of API testing using Postman. Key highlights include designing a mock API, employing advanced assertions, performing CRUD operations, integrating data-driven testing, and ensuring continuous testing with GitHub Actions and scheduling.

---

## ✨ Features

### 1️⃣ **Postman Collection**
- 🛠️ Created a Postman collection using a mock API.
- 📂 The collection focuses on endpoints for the `Booking` module.

### 2️⃣ **Advanced Assertions**
- ✅ Implemented validations for API responses:
  - JSON schema validation.
  - Date range checks.
  - Custom logic assertions.

### 3️⃣ **CRUD Operations**
- Verified core operations:
  - **Create**: Add new bookings.
  - **Read**: Retrieve booking details.
  - **Update**: Modify existing bookings.
  - **Delete**: Remove bookings.

### 4️⃣ **Data-Driven Testing**
- 📊 Integrated with an external data file for dynamic test inputs.
- 🔄 Ensured multiple data scenarios for exhaustive coverage.

### 5️⃣ **CI Integration with GitHub Actions**
- 🤖 Automated testing via GitHub Actions.
- 🛠️ Configured pipelines to run on repository changes.

### 6️⃣ **Performance Testing**
- 🚀 Evaluated performance of the collection `Booking env.postman_environment_xlr8.json`.
- 📈 Monitored response times and ensured API reliability under load.

### 7️⃣ **Environment Setup**
- 🗂️ Created an environment file `Booking env.postman_environment_xlr8.json`.
- 💾 Stored key variables like base URLs and API keys.

### 8️⃣ **Scheduling Collections**
- ⏰ Scheduled weekly collection runs.
- 🛡️ Monitored API health to detect potential issues early.

---

## 🛠️ Prerequisites
1. Install **Postman** (latest version).
2. Install **Node.js** for Newman CLI (if applicable).
3. Ensure a GitHub account with Actions enabled.

---

## 🚀 Installation and Setup
1. Clone this repository.
2. Import the Postman collection and environment file:
   - **Collection**: `Booking Collection.postman_collection.json`
   - **Environment**: `Booking env.postman_environment_xlr8.json`
3. Prepare the external data file for data-driven testing:
   - **File**: `testdata.csv`
4. Run the collection using Postman or Newman CLI:
   ```bash
   newman run "Booking Collection.postman_collection.json" -e "Booking env.postman_environment_xlr8.json" -d "testdata.csv"
