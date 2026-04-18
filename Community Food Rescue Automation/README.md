# ♻️ Community Food Rescue Automation

**Community Food Rescue Automation** is a smart workflow built in **n8n** that automatically connects **food donors** with **nearby volunteers** or **NGOs** in real time via **WhatsApp**.
The system reduces food waste and promotes community-driven sustainability by automating donation coordination and delivery.

---

## 📖 Overview

Every day, restaurants, canteens, and bakeries discard edible surplus food due to the lack of a coordinated donation system.
This project automates that process using **AI**, **automation**, and **real-time communication**.

When a donor sends a WhatsApp message about available food, the system:

1. Parses the message using **Google Gemini AI** to extract donation details.
2. Identifies the **pickup location** and matches it with **volunteers in the same city**.
3. Notifies eligible volunteers via WhatsApp.
4. Sends a confirmation to the donor once a volunteer accepts the task.

This creates an **end-to-end automated food rescue chain** that saves time and reduces waste.

---

## 🚀 Key Features

* 🤖 **AI-Powered Message Parsing** – Extracts food details (type, quantity, address, time) using Google Gemini.
* 🗺️ **Location-Based Volunteer Matching** – Detects pickup city and assigns available volunteers dynamically.
* 📲 **WhatsApp Automation** – Uses WhatsApp API for real-time communication with donors and volunteers.
* 📊 **Volunteer Database Integration** – Reads and updates volunteer records stored in Google Sheets.
* ⏳ **Automated Status Updates** – Notifies donors automatically once a volunteer confirms pickup.
* 🌱 **Zero Waste, Maximum Impact** – Enables sustainable redistribution of surplus food.

---

## 🧩 Workflow Components

| Component                                   | Description                                                                 |
| ------------------------------------------- | --------------------------------------------------------------------------- |
| **WhatsApp Trigger**                        | Captures incoming messages from donors via WhatsApp API.                    |
| **Command Detection**                       | Identifies key phrases like “food available” to route messages.             |
| **AI Parsing Node (Google Gemini)**         | Extracts structured data (food type, quantity, pickup address, etc.).       |
| **Data Processing (JavaScript Code Nodes)** | Cleans and structures the AI output into usable fields.                     |
| **Volunteer Database (Google Sheets)**      | Stores registered volunteers with details like city, capacity, and contact. |
| **City Matching Logic**                     | Matches the pickup city to available volunteers with remaining capacity.    |
| **Message Dispatch**                        | Sends pickup details to suitable volunteers via WhatsApp.                   |
| **Confirmation Handling**                   | Waits for volunteer response and updates the donor automatically.           |

<img width="1233" height="472" alt="workflow" src="https://github.com/user-attachments/assets/254aecef-a550-4e00-b92d-680d7f41e28c" />

---

## 🧰 Tech Stack

* **Workflow Platform:** n8n
* **AI Engine:** Google Gemini (PaLM API)
* **Database:** Google Sheets (Volunteer Records)
* **Messaging Platform:** WhatsApp Business API
* **Script Logic:** JavaScript (Custom Code Nodes)

---

## 🔄 Process Flow

1. **Donor Message Received:**
   Donor sends a WhatsApp message about food availability in Food donation WhatsApp group.
   
3. **Message Parsing:**
   Google Gemini extracts structured information.

4. **Volunteer Matching:**
   The system detects “Islamabad” from the pickup address and searches Google Sheets for active volunteers in that city.

5. **Notification Dispatch:**
   A WhatsApp message is sent to eligible volunteers with pickup details.

6. **Confirmation:**
   Once a volunteer accepts, the donor receives a WhatsApp confirmation.

---

## 📈 Impact

This project demonstrates how **AI and automation** can be leveraged for **social good**.
By integrating communication, intelligence, and logistics, it bridges the gap between **food surplus** and **food scarcity**, helping create a **zero-waste community ecosystem**.

---

**Areeba Bushra**
*Data Science & AI Enthusiast | Automation Developer*
📍 Based in Pakistan

