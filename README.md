# 🎮 DotaGuides – Android Application for Dota 2 Players

## 📌 Overview

DotaGuides is a mobile application developed in Kotlin for Android.
The app is designed to help players improve their gameplay by providing Up-to-date information about heroes, items, and matches.

It combines a local database, cloud storage, and external API to deliver real-time and structured game data.

Explanatory Note in russian: https://www.dropbox.com/scl/fi/r1oi1p191jxdmgkz7lcve/404.docx?rlkey=uxxtbwjkztvxe99ajvhb34wm5&st=ev8qaz5m&dl=0

---

## ⚙️ Technologies Used

* **Kotlin**
* **Android Studio**
* **MVVM Architecture**
* **Firebase Realtime Database**
* **Retrofit (OpenDota API)**
* **Room (local database)**

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

Data is stored in **JSON format**.

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

## 💡 Purpose

The project was developed as a diploma work to:

* design a mobile application
* work with APIs and cloud databases
* implement MVVM architecture
* improve Android development skills

