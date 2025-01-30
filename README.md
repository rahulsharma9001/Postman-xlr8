# Mastering Advanced API Testing with Postman: Automation, Dynamic Data, and Performance Testing

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
   - **File**: `Booking.csv`
4. Run the collection using Postman or Newman CLI:
   ```bash
   newman run "Booking Collection.postman_collection.json" -e "Booking env.postman_environment_xlr8.json" -d "Booking.csv"

## 🛠️ How to Use Monitors in Postman
Postman Monitors help automate API tests at scheduled intervals, ensuring API reliability over time. Follow these steps to set up and use monitors:

### 💡 Setting Up a Monitor
1. **Open Postman** and Navigate to your workspace.
2. Click in Monitors in the left-hand sidebar.
3. Click **Create a Monitor** and fill in the required details:
    - **Name:** Give your monitor a relevant name (e.g., Booking API Monitor).
    
    - **Collection:** Select the Booking Collection.postman_collection.json.
    
    - **Environment:** Choose Booking env.postman_environment_xlr8.json.
    
    - **Schedule:** Set the frequency of execution (e.g., every 24 hours, weekly).
    
    - **Regions:** Select a region closest to your API hosting server.
  
4. Click **Create Monitor** to save and activate it.

### 🔄 Running and Managing Monitors
  - **View Results:** Navigate to the Monitors tab to see execution history.
  
  - **Trigger a Manual Run:** Click on the monitor and press Run Monitor Now.
  
  - **Edit Settings:** Update the schedule, environment, or collection if needed.
  
  - **Notifications:** Enable email alerts or integrate with Slack for instant updates on API health.

### 🔧 Performing Performance Testing with Monitors
Postman Monitors can also be used for performance testing by tracking response times over scheduled runs. Steps to achieve this:

1. **Set Up a Monitor** for the Booking Collection.postman_collection.json.

2. **Enable Performance Metrics** under the monitor settings.

3. **Analyze Response Time Trends** over multiple runs.

4. **Identify Bottlenecks** and optimize API response times.
