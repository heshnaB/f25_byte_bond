# F25_C1

# ByteBond – Exam Deferral & Resource Management System
A partially functional Android application that demonstrates the UI, navigation flow, and limited offline/local data handling for an exam deferral and resource management system.

## Table of Contents
- [Overview](#overview)
- [Project Scope](#project-scope)
- [Features](#features)
- [Tech Stack](#tech-stack)
- [Project Structure](#project-structure)
- [Setup & Installation](#setup--installation)
- [Usage](#usage)
- [Testing](#testing)
- [Known Limitations](#known-limitations)
- [Future Work](#future-work)
- [Contributors](#contributors)

## Overview
This project is a partially functional Android application prototype designed to demonstrate the user interface, navigation flow, and limited data handling for an exam deferral and resource management system.

The project focuses primarily on front-end development and user experience, with some features supported by offline or local data storage. Full backend integration is not implemented for all workflows.

## Project Scope
### Included
- Front-end UI/UX implementation
- Role-based navigation (Student, Instructor, Administrator, and Proctor)
- Form input handling and validation
- Limited offline/local data support for select features

### Not Included / Partially Implemented
- Complete backend integration
- End-to-end data transfer across user roles
- Persistent storage for all features
- Messaging, notifications, and real-time updates
- Authentication and authorization

## Features
- Student exam deferral request interface
- Instructor exam configuration and upload screens
- Administrator room booking and scheduling UI
- Role-based screen flows
- Offline/local data handling for select screens

## Tech Stack
- Language: Kotlin
- Framework: Android Jetpack / Jetpack Compose
- IDE: Android Studio
- Build Tool: Gradle
- Version Control: Git & GitHub

## Project Structure
src/
├── androidTest/                    # Instrumented tests (Android device/emulator)
└── main/
    ├── java/
    │   └── com.example.myapplication/
    │       ├── data/               # Data layer (models, repositories, state)
    │       │   ├── firebase/       # Firebase-related data access/helpers
    │       │   ├── repository/     # Repository classes (data sources)
    │       │   ├── viewmodels/     # ViewModels / UI state holders
    │       │   └── README.md       # Notes/docs for the data layer
    │       │
    │       ├── logic/              # App/business logic by feature
    │       │   ├── auth/           # Authentication logic
    │       │   ├── messaging/      # Messaging feature logic
    │       │   ├── notification/   # Notifications feature logic
    │       │   ├── scheduling/     # Scheduling feature logic
    │       │   ├── utils/          # Shared utilities/helpers
    │       │   └── README.md       # Notes/docs for the logic layer
    │       │
    │       ├── ui.theme/           # UI layer (screens, navigation, theme)
    │       │   ├── adminDashb/     # Admin dashboard screens/components
    │       │   ├── proctorDashb/   # Proctor dashboard screens/components
    │       │   ├── professorDashb/ # Professor dashboard screens/components
    │       │   ├── studentDashb/   # Student dashboard screens/components
    │       │   ├── button.kt
    │       │   ├── Color.kt
    │       │   ├── LoginScreen.kt
    │       │   ├── MainDashboard.kt
    │       │   ├── MainInbox.kt
    │       │   ├── MainLayout.kt
    │       │   ├── NavGraph.kt     # Navigation graph/routes
    │       │   ├── RealTimeStatusListener
    │       │   ├── SelectUserType.kt
    │       │   ├── Theme.kt
    │       │   └── Type.kt
    │       │
    │       └── MainActivity.kt     # App entry point
    │
    └── res/                        # Android resources (drawables, values, etc.)

## Setup & Installation
1. Clone the repository
2. Open the project in Android Studio
3. Start an Android emulator or connect a physical device
4. Allow Gradle to sync
5. Run the application

## Usage
The application is intended as a prototype.

Users can navigate through different roles, interact with UI components, and observe the intended workflow. Some data is handled locally, but not all features persist data or synchronize across roles.

## Data Support
This project includes limited offline or local data handling for select features. Not all user inputs or uploads persist across sessions, and some workflows remain UI-only.

## Testing
- Manual UI testing performed
- Navigation and layout consistency verified
- Button interactions tested
- Automated testing not implemented due to project scope

## Known Limitations
- Partial backend or local data support
- Incomplete data flow between roles
- Some features reset when the app restarts
- File uploads may be UI-only

## Future Work
- Full backend and database integration
- Cross-role data synchronization
- Authentication and authorization
- Automated testing
- APK deployment

## Contributors
- Front-end development, UI/UX design, navigation, testing, and documentation — Heshna B
- Backend setup and partial data handling — Project contributor
