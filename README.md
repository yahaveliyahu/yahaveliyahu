# 👋 Hi, I'm Yahav Eliyahu

## About

Results-driven software developer with a strong academic foundation in Computer Science and extensive hands-on experience in mobile development, machine learning, cybersecurity, and cloud technologies.

Skilled in developing high-quality, user-focused Android and iOS applications with strong attention to architecture, performance, and seamless user experience, including experience in computer vision and AI-driven features.

Beyond software development, I have a growing professional focus on cybersecurity. My background includes network security fundamentals, secure communication protocols, threat detection concepts, vulnerability analysis, and hands-on exposure to defensive tools and methodologies.

Demonstrated ability to learn quickly, solve complex technical challenges, and lead projects from concept to production. Combining creativity, analytical thinking, and a passion for clean architecture, I strive to develop impactful projects while keeping performance, UX, and security in mind.

Looking to contribute and grow in a cybersecurity or development role, particularly in AppSec or mobile development.

--- 

## 🔐 Cybersecurity Portfolio

📁 Hands-on cybersecurity labs, write-ups, and learning progress  
focused on SOC operations, SIEM & log analysis, threat frameworks (MITRE ATT&CK, Cyber Kill Chain), networking, Windows & Active Directory, Linux, and web security.

👉 <img src="https://cdn.jsdelivr.net/gh/devicons/devicon/icons/github/github-original.svg" width="18"/>
[View my Cybersecurity Portfolio](https://github.com/yahaveliyahu/Cyber-portfolio)

--- 

## 🔥 Featured Projects

### 🔐 AntiPhishing – Cross-app phishing detection system (Kotlin, Swift, Flask, XGBoost)

📱 [Android App (Kotlin)](https://github.com/yahaveliyahu/AntiPhishing-Android.git) · 🍎 [iOS App (Swift)](https://github.com/yahaveliyahu/AntiPhishing-IOS.git) · 🖥️ [Backend (Python, Flask, XGBoost)](https://github.com/yahaveliyahu/AntiPhishing-Server.git)

Mobile security system that intercepts links from any app (SMS/WhatsApp/Browser) and evaluates them before opening, combining on-device lexical analysis with server-side ML scoring to generate a real-time risk percentage and user-friendly explanation. Features zero-day detection pipeline, Intent-based interception, caching + threat intelligence lookup, and explainable alerts with blocking for high-risk links.

- **Android (Kotlin, Jetpack Compose, Hilt, multi-module Gradle):** system-wide link interception, CameraX + ML Kit QR scanning, and an on-device lexical engine running 74 checks to build a 52-feature vector, with results cached in Room.
- **iOS (Swift, SwiftUI):** Safari Web Extension, Share Extension and QR scanner, backed by an offline SQLite database of 600K+ malicious domains so lookups never leave the device.
- **Backend (Python, Flask, XGBoost):** MongoDB Atlas threat database seeded from 20+ public threat-intelligence feeds; unknown URLs are scored by an XGBoost model (57 features, trained on 1.7M+ URLs, 96.1% accuracy). Dockerized, served by Gunicorn and continuously deployed on Render.

### 📡 **StreamBridge — Secure Phone-to-PC Communication System**

📱 [Android Server (Kotlin)](https://github.com/yahaveliyahu/StreamBridge-Android.git)

Real-time secure communication server with a Windows client over LAN. Implements live camera streaming (CameraX) over WSS, built on NanoHTTPD. Implements TLS with ECDHE, ECDSA, and AES-256-GCM encryption, TOFU-based pairing with certificate pinning. Supports file transfer, bidirectional messaging, remote photo capture and Integrated local network discovery (mDNS / JmDNS) for automatic device detection.

💻 [Windows Client (Kotlin + JavaFX)](https://github.com/yahaveliyahu/StreamBridge-Windows.git)

A Desktop client application for interacting with the Android server over LAN. Built a responsive UI for live stream viewing, chat and file management. Includes secure HTTPS/WSS communication, encrypted data handling and real-time media rendering. Developed auto-discovery of devices using mDNS and QR-based pairing workflow. Packaged as a native Windows installer (.exe) with jpackage.

### 🍽️ [KitchenMate — Smart Android Recipe Assistant (Kotlin, Firebase, ML)](https://github.com/yahaveliyahu/KitchenMate.git)

End-to-end Android app for discovering recipes based on available ingredients, featuring on-device ingredient recognition (TensorFlow Lite), barcode scanning (ZXing), OCR-based recipe import from photos and PDFs (ML Kit Text Recognition, Tesseract), and a multi-step matching pipeline combining Firestore and Spoonacular APIs with intelligent fallback. Includes caching + coroutines optimization, favorites/history system, and admin approval workflow.

### 📅 [MyCalendar – Android calendar library with a Hebrew calendar engine (Kotlin, Jetpack Compose)](https://github.com/yahaveliyahu/MyCalendar.git)

Android calendar library built on a from-scratch implementation of Hebrew calendar arithmetic: molad-based Hebrew↔Gregorian conversion, gematria numerals, and a complete Jewish holiday calendar with real postponement rules, unit-tested against Hebcal and Chabad.org reference dates. A three-module library: a pure-Kotlin core with zero Android dependencies, a Canvas-drawn custom month View, and a Jetpack Compose demo app with Month, Week, Day and Year views, exact-time reminders (AlarmManager), daily holiday notifications (WorkManager) and RFC 5545 .ics sharing.

### 🏃 [FitnessTracker – Two fitness apps on one shared library (Kotlin, Jetpack Compose, Room)](https://github.com/yahaveliyahu/Fitnesstracker.git)

Multi-module Android project with two apps — RunTracker and CycleTracker — built on a single shared :common library, so each app is only a configuration object (sport type, colors, MET value). Live GPS tracking (FusedLocationProviderClient), step detection, calorie estimation, coaching milestones, personal-best detection and weekly goals, with Room persistence, MVVM and a Material 3 Compose UI.

### 🖼️ [GuessThePic – iOS picture-guessing game (Swift, SwiftUI)](https://github.com/yahaveliyahu/GuessThePic.git)

Original iOS game in pure SwiftUI: a hidden photo is revealed pixel by pixel on a Canvas while the score decays from 1000 to 100, so every second makes the guess easier but worth less. Friend challenges work with zero backend — the whole challenge is encoded in a deep link plus a short fallback code and shared as a ready-to-send WhatsApp message. Built with MVVM, Swift Concurrency (Task-based timer, @MainActor), a protocol-based leaderboard service, and a shareable leaderboard card rendered as an image.

### 📚 [City Library Management System – PostgreSQL database with business rules in SQL](https://github.com/yahaveliyahu/City-library-management-system.git)

PostgreSQL database for a multi-branch city library (9 tables, normalized to 3NF) where the business rules are enforced inside the database rather than in application code: partial unique indexes, CHECK constraints, BEFORE/AFTER triggers that block invalid loans and generate late fines automatically, reporting views, and a PL/pgSQL renew_loan() function with exception handling. One-command setup with Docker Compose.

### 🧹 [CleanTrack – Job-ticket app for a cleaning company (React Native, Expo)](https://github.com/yahaveliyahu/CleanTrack.git)

Cross-platform mobile app where any staff member can open a cleaning job ticket, and a ticket can only be closed after a photo is taken on the spot as proof of completed work. Includes active and history views with search and status filters, a full-screen photo lightbox, and local persistence with AsyncStorage. Android APK built with EAS Build.

### 🎮 [SurviveGameFixed – Reverse engineered Android game rebuild (APK → Android Studio)](https://github.com/yahaveliyahu/SurviveGameFixed.git)

Reconstructed a fully working Android game starting from a broken APK with no source code, performing full decompilation, project rebuilding (code/resources/Gradle), and systematic debugging to restore functionality. Fixed critical issues including hidden-character URL bugs, network permissions, dependency/SDK mismatches, and UI interaction problems, resulting in a verified working app on a physical device.

### 📱 [Context-Aware Login – Multi-factor environmental authentication (Android, ML Kit)](https://github.com/yahaveliyahu/Context-Aware-Login.git)

Smart authentication app that grants access only when multiple real-world conditions are met, combining system signals and sensor data (battery, WiFi, Bluetooth, microphone, and camera) with ML-based smile detection. Implements coroutine-based validation pipeline with detailed failure feedback and integrates diverse Android APIs for context-aware security.

### 🃏 [War Game Cards – iOS card game (Swift, UIKit)](https://github.com/yahaveliyahu/War-game.git)

Two-player iOS card game built with UIKit, Storyboard and Auto Layout: 10 timed rounds against the computer with card-flip animations and full War tie-breaking rules, Core Location to assign the player to the East or West side, and AVFoundation audio (background music, card-flip, war and victory sounds).

### 🚀 [Asteroid Avoidance Game – Android arcade game with sensors & maps (Kotlin, Google Maps)](https://github.com/yahaveliyahu/Asteroid-Avoidance-Game.git)

Lane-based arcade game where players dodge obstacles using touch or accelerometer controls, featuring dynamic difficulty scaling, boost/brake mechanics, and collision-based feedback (sound + vibration). Includes high-score system with tracking  GPS location, Google Maps integration for score visualization, and persistent storage using SharedPreferences + Gson.

### 🌍 [Israeli Passport Quiz – Android quiz game with lives system (Kotlin)](https://github.com/yahaveliyahu/IsraeliPassportQuiz.git)

Interactive quiz app that challenges users to identify travel eligibility by country using flag-based questions, featuring score tracking, heart-based lives system, dark mode support, and end-game states with replay functionality.

### 🛒 [ShopSystem – Retail management system in pure C](https://github.com/yahaveliyahu/ShopSystem.git)

Built retail shop management system covering products, employees, customers with shopping carts, category shelves and reviews. Hand-built data structures — a generic void* linked list, a doubly linked list with O(1) removal, and function-pointer-driven generic routines with qsort/bsearch — plus manual memory management verified leak-free with AddressSanitizer, and save/load in both text and a custom compressed binary format.

### 🦁 [Zoo Management System – Java OOP + PostgreSQL (JDBC)](https://github.com/yahaveliyahu/Zoo-Management-System-Java-OOP-with-PostgreSQL-database.git)

Object-oriented Java application modeling a zoo system using inheritance, polymorphism, and custom comparators, with full PostgreSQL integration for persistent storage and querying via JDBC. Implements animal lifecycle management, sorting/filtering logic, and structured DB operations with a layered design (manager + connector).

### 🏦 [Bank System – Java OOP design with SOLID principles](https://github.com/yahaveliyahu/BankSystem-Java-OOP.git)

Console-based banking system implementing core OOP concepts (inheritance, polymorphism, encapsulation) and SOLID principles, featuring multiple account types, factory-based object creation, and custom exception handling for robust client/account management.

---

## 🛠️ Technologies & Tools

### **Languages**
<p align="left">
  <img src="https://cdn.jsdelivr.net/gh/devicons/devicon/icons/kotlin/kotlin-original.svg" width="45" title="Kotlin" alt="Kotlin" />
  <img src="https://cdn.jsdelivr.net/gh/devicons/devicon/icons/java/java-original.svg" width="45" title="Java" alt="Java" />
  <img src="https://cdn.jsdelivr.net/gh/devicons/devicon/icons/swift/swift-original.svg" width="45" title="Swift" alt="Swift" />
  <img src="https://cdn.jsdelivr.net/gh/devicons/devicon/icons/python/python-original.svg" width="45" title="Python" alt="Python" />
  <img src="https://cdn.jsdelivr.net/gh/devicons/devicon/icons/c/c-original.svg" width="45" title="C" alt="C" />
  <img src="https://cdn.jsdelivr.net/gh/devicons/devicon/icons/javascript/javascript-original.svg" width="45" title="JavaScript" alt="JavaScript" />
</p>

### **Mobile**
<p align="left">
  <img src="https://cdn.jsdelivr.net/gh/devicons/devicon/icons/android/android-plain.svg" width="45" title="Android" alt="Android" />
  <img src="https://cdn.jsdelivr.net/gh/devicons/devicon/icons/jetpackcompose/jetpackcompose-original.svg" width="45" title="Jetpack Compose" alt="Jetpack Compose" />
  <img src="https://cdn.jsdelivr.net/gh/devicons/devicon/icons/react/react-original.svg" width="45" title="React Native" alt="React Native" />
  <img src="https://cdn.jsdelivr.net/gh/devicons/devicon/icons/expo/expo-original.svg" width="45" title="Expo" alt="Expo" />
</p>

### **Backend & Databases**
<p align="left">
  <img src="https://cdn.jsdelivr.net/gh/devicons/devicon/icons/flask/flask-original.svg" width="45" title="Flask" alt="Flask" />
  <img src="https://cdn.jsdelivr.net/gh/devicons/devicon/icons/firebase/firebase-plain.svg" width="45" title="Firebase" alt="Firebase" />
  <img src="https://cdn.jsdelivr.net/gh/devicons/devicon/icons/mongodb/mongodb-original.svg" width="45" title="MongoDB" alt="MongoDB" />
  <img src="https://cdn.jsdelivr.net/gh/devicons/devicon/icons/postgresql/postgresql-original.svg" width="45" title="PostgreSQL" alt="PostgreSQL" />
  <img src="https://cdn.jsdelivr.net/gh/devicons/devicon/icons/sqlite/sqlite-original.svg" width="45" title="SQLite" alt="SQLite" />
</p>

### **Machine Learning & Data**
<p align="left"> 
  <img src="https://cdn.jsdelivr.net/gh/devicons/devicon/icons/tensorflow/tensorflow-original.svg" width="45" title="TensorFlow Lite" alt="TensorFlow" />
  <img src="https://cdn.jsdelivr.net/gh/devicons/devicon/icons/scikitlearn/scikitlearn-original.svg" width="45" title="scikit-learn" alt="scikit-learn" />

### **Tools & Platforms**
<p align="left">
  <!-- Version Control -->
  <img src="https://cdn.jsdelivr.net/gh/devicons/devicon/icons/git/git-original.svg" width="45" />
  <img src="https://cdn.jsdelivr.net/gh/devicons/devicon/icons/github/github-original.svg" width="45" />
  <img src="https://cdn.jsdelivr.net/gh/devicons/devicon/icons/pandas/pandas-original.svg" width="45" title="pandas" alt="pandas" /> 
</p>

### **Security & Systems**
  <p align="left"> 
    <img src="https://cdn.jsdelivr.net/gh/devicons/devicon/icons/linux/linux-original.svg" width="45" title="Linux" alt="Linux" />
    <img src="https://cdn.jsdelivr.net/gh/devicons/devicon/icons/windows11/windows11-original.svg" width="45" title="Windows" alt="Windows" />
    <img src="https://cdn.jsdelivr.net/gh/devicons/devicon/icons/powershell/powershell-original.svg" width="45" title="PowerShell" alt="PowerShell" />
    <img src="https://gitlab.com/wireshark/wireshark/-/raw/master/resources/icons/wsicon128.png" width="45" title="Wireshark" alt="Wireshark" /> 
  </p>

### **DevOps & Tools**
<p align="left"> 
  <img src="https://cdn.jsdelivr.net/gh/devicons/devicon/icons/git/git-original.svg" width="45" title="Git" alt="Git" />
  <img src="https://cdn.jsdelivr.net/gh/devicons/devicon/icons/github/github-original.svg" width="45" title="GitHub" alt="GitHub" />
  <img src="https://cdn.jsdelivr.net/gh/devicons/devicon/icons/docker/docker-original.svg" width="45" title="Docker" alt="Docker" />
  <img src="https://cdn.jsdelivr.net/gh/devicons/devicon/icons/gradle/gradle-original.svg" width="45" title="Gradle" alt="Gradle" />
  <img src="https://www.vectorlogo.zone/logos/getpostman/getpostman-icon.svg" width="45" title="Postman" alt="Postman" />
  <img src="https://cdn.jsdelivr.net/gh/devicons/devicon/icons/vercel/vercel-original.svg" width="45" title="Vercel" alt="Vercel" />
  <img src="https://cdn.jsdelivr.net/gh/devicons/devicon/icons/unity/unity-original.svg" width="45" title="Unity" alt="Unity" />
</p>
  
  <!-- IDEs -->
  <p align="left"> 
  <img src="https://cdn.jsdelivr.net/gh/devicons/devicon/icons/androidstudio/androidstudio-original.svg" width="45" title="Android Studio" alt="Android Studio" />
  <img src="https://cdn.jsdelivr.net/gh/devicons/devicon/icons/xcode/xcode-original.svg" width="45" title="Xcode" alt="Xcode" />
  <img src="https://cdn.jsdelivr.net/gh/devicons/devicon/icons/intellij/intellij-original.svg" width="45" title="IntelliJ IDEA" alt="IntelliJ IDEA" />
  <img src="https://cdn.jsdelivr.net/gh/devicons/devicon/icons/pycharm/pycharm-original.svg" width="45" title="PyCharm" alt="PyCharm" />
  <img src="https://cdn.jsdelivr.net/gh/devicons/devicon/icons/clion/clion-original.svg" width="45" title="CLion" alt="CLion" />
  <img src="https://cdn.jsdelivr.net/gh/devicons/devicon/icons/vscode/vscode-original.svg" width="45" title="VS Code" alt="VS Code" />
  <img src="https://cdn.jsdelivr.net/gh/devicons/devicon/icons/visualstudio/visualstudio-plain.svg" width="45" title="Visual Studio" alt="Visual Studio" />
</p>

---

## Connect With Me

<p align="left">
  <a href="https://www.linkedin.com/in/yahav-eliyahu-9a07a8334">
    <img src="https://cdn.jsdelivr.net/gh/devicons/devicon/icons/linkedin/linkedin-original.svg" width="45" style="margin-right: 15px;" />
  </a>
  <a href="mailto:yahaveliyahu@gmail.com">
      <img src="https://upload.wikimedia.org/wikipedia/commons/thumb/7/7e/Gmail_icon_%282020%29.svg/240px-Gmail_icon_%282020%29.svg.png" width="45" /> 
  </a>
</p>




