Business Card App

Android application developed as a coursework project using Kotlin and Jetpack Compose.
The app provides a clean business card interface with navigation to CV, portfolio, settings, and contact form.
User preferences and CV entries are stored locally using DataStore.

Features
1. Business Card Screen

Displays personal information:

Profile photo

Name and job title

Email and phone number

Navigation to all sections

2. CV Section

Includes:

Static "About Me" section

Skills list

Dynamic CV item management:

Add new CV items

Delete existing items

All data is saved locally using DataStore

3. Portfolio Section

Displays portfolio projects with:

Project image

Description

External link to Behance (opens via system browser)

4. Settings

The user can change the application language:

English

Russian

Language is stored in DataStore and applied globally through recreation of the activity.

5. Contact Form

A simple contact page where user can:

Enter name, email, and message

Send the message via the device’s email client (using Intent.ACTION_SENDTO)
No data is sent automatically or stored remotely.

Technologies Used

Kotlin

Jetpack Compose

Material 3

Coil (image loading)

DataStore Preferences (persistent storage)

Navigation Compose

AndroidX Libraries

Project Structure
/MainActivity.kt
/Navigation.kt
/ui/theme
/data
    AppDataStore.kt
    CVRepository.kt
    Models.kt
/screens
    BusinessCard.kt
    CV.kt
    ContactForm.kt
    Portfolio.kt
    Settings.kt
/components
    Components.kt

Data Storage

The application uses DataStore Preferences to persist:

Selected language

CV items

All stored information remains on the device only.

Privacy Policy

The application does not collect, store, transmit, or share any personal data.
All information added by the user is stored locally.
The app does not use camera, microphone, location, or network communication for data collection.

Full policy: see PRIVACY_POLICY.md

Terms and Conditions

The application is provided for educational purposes.
The developer is not responsible for incorrect input or data loss.
All data is stored locally using Android DataStore.

Full terms: see TERMS_AND_CONDITIONS.md

How to Run

Clone the repository

Open the project in Android Studio Hedgehog or newer

Sync Gradle

Run on an Android device or emulator (minSdk = 24)

Requirements

Android Studio Hedgehog (or newer)

Android device or emulator running Android 7.0+

Internet connection (only for loading portfolio images)
