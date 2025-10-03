# IoMT-StressEase-App
Mobile health app StressEase built with Flutter + AWS (Lambda, DynamoDB, API Gateway) integrating Fitbit API to monitor stress via self-reports + wearables. Features secure login, stress check-ins, real-time sync, cloud storage, and dashboards for stress insights.
# 🌐 StressEase – IoMT-Based Stress Monitoring App  

A mobile health app designed to **monitor and manage stress** by integrating **self-reported inputs** with **wearable data** from Fitbit devices. Built with **Flutter frontend**, **AWS backend (Lambda, API Gateway, DynamoDB)**, and **Fitbit API** for real-time physiological data.  

---

## 📌 Project Overview  
- **Problem:** Stress is under-monitored; patients lack tools to track it in real-time.  
- **Solution:** IoMT-based system combining **self-reports + wearable metrics** into a single app.  
- **Impact:** Provides **personalized insights**, encourages self-awareness, and supports proactive stress management.  

---

## 🚀 System Architecture  

### Frontend – Flutter App  
- Secure login & signup  
- Daily stress check-ins (emoji-based + notes)  
- Connect & sync Fitbit devices  
- Stress insights dashboards (self-reported vs Fitbit metrics)  

### Backend – AWS Cloud  
- **API Gateway:** Handles secure HTTP requests  
- **AWS Lambda:** Functions for Fitbit data fetch, token refresh, and stress data storage  
- **DynamoDB:** Stores user stress logs and Fitbit data  

### Third-Party – Fitbit API  
- **OAuth 2.0 integration** for secure wearable data access  
- Fetches heart rate, sleep, activity levels  
- Refreshes tokens to maintain continuous sync  

---

## 📊 Component Workflow  
1. User logs in and records stress or syncs Fitbit data.  
2. App sends requests via **API Gateway**.  
3. **Lambda functions** fetch data from Fitbit or save to DynamoDB.  
4. Results returned to app, displayed in Flutter UI with charts and reports.  

---

## 💡 Key Features  
- **Daily Stress Check-In** (emoji UI + notes)  
- **Fitbit Sync** (heart rate, sleep, steps)  
- **Dynamic Reports** (compare self-reported vs measured stress)  
- **Scalable AWS backend** (serverless, cloud-native)  
- **Secure Data Handling** (OAuth2, token refresh, DynamoDB storage)  

---

## 📊 Results & Insights  
- Successfully implemented **OAuth 2.0 Fitbit integration**  
- Built fully **serverless backend** with AWS Lambda + DynamoDB  
- Delivered **real-time stress monitoring** app tested on emulators  
- Overcame challenges with OAuth, token refresh, and frontend-backend communication  

---

## ⚡ Challenges & Solutions  
- **OAuth 2.0 Flow:** Solved via Postman testing & Base64 credential encoding.  
- **API Integration:** Modular Lambda functions tested individually before integration.  
- **UI Consistency:** Used Flutter navigation routes + stateful widgets for reliability.  

---

## 🔮 Future Enhancements  
- Add **machine learning models** for predictive stress alerts  
- Expand wearable integration (Apple Watch, Garmin)  
- Enable **data export for clinicians**  
- Deploy as a **public health IoMT platform**  

---
