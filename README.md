# 🩺 MedSync

**MedSync** is a dual mobile application system designed to seamlessly connect **doctors** and **patients**.
It enables doctors to upload prescriptions, while patients receive **automated medicine reminders** and updates — making healthcare management simple, accessible, and especially user-friendly for the elderly.

***

## 🚀 Project Overview

MedSync bridges the communication gap between doctors and patients by synchronizing prescriptions, reminders, and medication schedules through a shared digital platform.

### 👨‍⚕️ Doctor App

- Upload and update prescriptions
- Schedule medicine reminders for patients
- Track patient progress


### 👩‍🦳 Patient App

- Receive reminders to buy and take medicines
- View prescriptions and dosage details
- Simple UI designed for elderly and non-tech-savvy users

***

## 🛠️ Tech Stack

| Layer | Technology |
| :-- | :-- |
| **Frontend** | React Native (Expo) |
| **Backend** | Firebase (Authentication, Firestore Database, Storage) |
| **Language** | JavaScript / TypeScript |
| **Version Control** | Git + GitHub |
| **Design Tools** | Figma (for UI/UX prototyping) |


***

## 📱 Features Roadmap

### ✅ **Phase 1 — Semester 1 (30%)**

> Focus on setup, authentication, and UI foundation.

- [x] Firebase integration
- [x] Authentication (Sign Up / Log In)
- [x] Basic UI for Login, Doctor, and Patient Screens
- [ ] Navigation between screens


### 🚧 **Phase 2 — Semester 2 (Remaining 70%)**

> Focus on core functionality and polish.

- [ ] Prescription upload (Doctor side)
- [ ] Medicine reminder system (Patient side)
- [ ] Notification support
- [ ] Profile management
- [ ] Cloud Firestore database linking
- [ ] Final testing and optimization

***

## ⚙️ Installation \& Setup

### 1️⃣ Clone the Repository

```bash
git clone https://github.com/<your-username>/MedSync.git
cd MedSync
```


### 2️⃣ Install Dependencies

```bash
npm install
```


### 3️⃣ Configure Firebase

Create a file at `src/firebase/config.js` and add your Firebase credentials:

```javascript
// src/firebase/config.js
import { initializeApp } from "firebase/app";
import { getAuth } from "firebase/auth";

const firebaseConfig = {
  apiKey: "YOUR_API_KEY",
  authDomain: "your-app.firebaseapp.com",
  projectId: "your-app-id",
  storageBucket: "your-app.appspot.com",
  messagingSenderId: "YOUR_SENDER_ID",
  appId: "YOUR_APP_ID"
};

const app = initializeApp(firebaseConfig);
export const auth = getAuth(app);
```

**Tip:** Keep your actual Firebase keys out of GitHub by using environment variables or a `.env` file (and add `.env` to `.gitignore`).

### 4️⃣ Run the App

```bash
npx expo start
```


***

## 🤝 Contributing

1. Fork / clone the repo
2. Create a feature branch

```bash
git checkout -b feature/<feature-name>
```

3. Commit and push changes

```bash
git add .
git commit -m "Added <feature-name>"
git push origin feature/<feature-name>
```

4. Create a Pull Request (PR) to `dev` branch
5. After review, merge `dev` → `main` when stable

***

## 📋 Git Workflow

- **main** → stable, production-ready code
- **dev** → ongoing development
- **feature/...** → specific feature branches (e.g., `feature/login`, `feature/reminders`)

***

## 🧩 Future Enhancements

- AI-based medicine recognition via image scanning
- Integration with pharmacies for auto-refill reminders
- Health report generation and analytics

***

## 🧑‍💻 Team Members

| Name | Role |
| :-- | :-- |
| Swayam Ruparel | Frontend \& Firebase Integration |
| Clint Loyed | UI/UX Design |
| Rohit Xavier | Backend Integration |
| Aryan Reshi | Documentation \& Testing |


***

## 📄 License

This project is licensed under the MIT License — feel free to use and modify it for educational purposes.

***

🌿 *"Simplifying healthcare, one sync at a time."*

