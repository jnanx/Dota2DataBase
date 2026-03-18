# 🎮 DotaGuides – Android Application for Dota 2 Players

## 📌 Overview

DotaGuides is a mobile application developed in Kotlin for Android.
The app is designed to help players improve their gameplay by providing актуальную информацию о героях, предметах и матчах.

It combines a local database, cloud storage, and external API to deliver real-time and structured game data.

---

## ⚙️ Technologies Used

* **Kotlin**
* **Android Studio**
* **MVVM Architecture**
* **Firebase Realtime Database**
* **Retrofit (OpenDota API)**
* **Room (local database)**
* **RecyclerView**

---

## 🏗️ Architecture

The application follows the **MVVM (Model-View-ViewModel)** pattern:

* **Model** – data classes (Hero, Item, Match, Player)
* **View** – UI (Activities, Fragments)
* **ViewModel** – business logic and data handling

The project also includes a **Repository layer** for managing data sources.

---

## 🌐 Data Sources

### 🔹 Firebase

Used for storing:

* heroes
* items
* abilities
* talents

Data is stored in **JSON format** and loaded in real time.

---

### 🔹 OpenDota API

Used for:

* fetching match data
* retrieving professional matches

---

### 🔹 Room Database

Used for:

* caching match data locally
* reducing API calls
* offline access

---

## 🚀 Features

### 🧙‍♂️ Heroes and Items

* Browse heroes and items
* View detailed information (abilities, stats, etc.)
* Search by name

---

### ⏱️ Timers

* Track important in-game events

---

### 🎮 Pro Matches

* View matches of professional players
* Filter by selected hero

---

### 🔎 Match Search

* Search match by ID
* View detailed statistics:

  * players
  * items
  * match results

---

## 🔄 Application Flow

1. User interacts with UI
2. ViewModel processes the action
3. Repository fetches data:

   * from Firebase (static data)
   * from API (dynamic data)
4. Data is mapped (DTO → Model)
5. UI is updated

---

## 🧪 Development Process

The application was developed in several stages:

* Data collection and API research
* Firebase database creation and JSON import
* UI design (Figma)
* Implementation in Android Studio
* Integration of Retrofit, Room, Firebase
* MVVM structure implementation
* Feature development (search, timers, matches)

---

## 🔐 Requirements

### Software

* Android Studio (Flamingo or newer)
* Android SDK

### Device

* Android 8.1 or higher
* Internet connection required

---

## 💡 Purpose

The project was developed as a diploma work to:

* design a mobile application
* work with APIs and cloud databases
* implement MVVM architecture
* improve Android development skills

---

## 🚀 Future Improvements

* Better UI/UX
* Improved caching system
* Error handling and loading states
* Additional filters and analytics

---

## 👩‍💻 Author

Maria Samar
