# Permissions Score

[![Android](https://img.shields.io/badge/Platform-Android-green.svg)](https://developer.android.com)
[![Kotlin](https://img.shields.io/badge/Language-Kotlin-purple.svg)](https://kotlinlang.org)
[![Compose](https://img.shields.io/badge/UI-Compose-orange.svg)](https://developer.android.com/jetpack/compose)

An Android application designed to assess and enhance device security by analyzing app permissions and providing actionable security scores. This app helps users understand their device's security posture through comprehensive permission analysis and device security checks.

## 📋 Table of Contents

- [Features](#features)
- [Screenshots](#screenshots)
- [Installation](#installation)
- [Usage](#usage)
- [Architecture](#architecture)
- [Technology Stack](#technology-stack)
- [Contributing](#contributing)
- [Credits](#credits)
- [License](#license)

## ✨ Features

### 🔒 Security Assessment
- **Overall Security Score**: Comprehensive score out of 100 based on multiple security factors
- **Device Security**: Checks PIN/password lock and biometric authentication status
- **App Permission Analysis**: Categorizes permissions into High, Moderate, and Low sensitivity levels
- **Third-Party App Detection**: Identifies apps not installed from Google Play Store

### 📱 User Interface
- **Material 3 Design**: Modern, intuitive interface built with Jetpack Compose
- **Animated Dashboard**: Smooth animations and transitions for enhanced user experience
- **Dark Theme**: Eye-friendly dark theme with gradient backgrounds
- **Responsive Navigation**: Bottom navigation with multiple screens

### 📊 Detailed Analytics
- **Permission Breakdown**: Detailed view of apps using sensitive permissions
- **Score Categories**: Visual representation of security levels (Danger, Weak, Moderate, Safe, Protected)
- **Real-time Updates**: Dynamic score calculation based on current device state

### 🛠️ Additional Features
- **App Management**: View and analyze installed applications
- **Notification Center**: Manage app notification permissions
- **Settings**: Customize permission sensitivity levels
- **Categories View**: Group apps by permission usage patterns

## 📸 Screenshots

*Screenshots will be added soon*

## 🚀 Installation

### Prerequisites
- **Android Studio**: Arctic Fox or later
- **Minimum SDK**: API 24 (Android 7.0)
- **Target SDK**: API 34 (Android 14)
- **Kotlin**: 1.8+

### Setup Instructions

1. **Clone the repository**
   ```bash
   git clone https://github.com/your-username/permissions-score.git
   cd permissions-score
   ```

2. **Open in Android Studio**
   - Launch Android Studio
   - Select "Open an existing Android Studio project"
   - Navigate to the cloned directory and select it

3. **Configure Firebase (Optional)**
   - Add your `google-services.json` file to the `app/` directory
   - This enables analytics and data upload features

4. **Build the project**
   - Wait for Gradle sync to complete
   - Build → Make Project (Ctrl+F9)

5. **Run on device/emulator**
   - Connect an Android device or start an emulator
   - Run → Run 'app' (Shift+F10)

### Alternative Build (Command Line)
```bash
# Build APK
./gradlew assembleDebug

# Install on connected device
./gradlew installDebug
```

## 📖 Usage

### Getting Started
1. **Launch the App**: Open Permissions Score on your Android device
2. **Grant Permissions**: Allow necessary permissions for app analysis
3. **View Dashboard**: Check your overall security score on the home screen

### Understanding Your Score
- **0-30**: Danger - Immediate action needed
- **31-50**: Weak - Needs improvement
- **51-70**: Moderate - Basic protection
- **71-90**: Safe - Generally protected
- **91-100**: Protected - Excellent security

### Navigating Features
- **Home**: Security dashboard and overall score
- **Apps**: List and analyze installed applications
- **Notifications**: Manage notification permissions
- **Settings**: Configure permission sensitivities
- **Categories**: View apps grouped by permission usage

## 🏗️ Architecture

The app follows modern Android development practices:

```
app/
├── src/main/java/com/dubd/permissionsscore/
│   ├── MainActivity.kt          # Main activity with navigation
│   ├── HomeScreen.kt            # Security dashboard
│   ├── AppsScreen.kt            # App listing and analysis
│   ├── CategoriesScreen.kt      # Permission-based categorization
│   ├── SettingsScreen.kt        # User preferences
│   ├── PermissionsSensitivityScreen.kt  # Permission configuration
│   ├── NotificationsScreen.kt   # Notification management
│   ├── DataManager.kt           # Data initialization
│   ├── PermissionsPreferences.kt # Permission settings
│   ├── UploadHelper.kt          # Firebase data upload
│   ├── viewmodel/
│   │   └── AppViewModel.kt      # UI state management
│   └── ui/theme/                # Material 3 theming
├── src/main/res/                # Resources (layouts, drawables, values)
└── src/main/AndroidManifest.xml  # App manifest
```

## 🛠️ Technology Stack

### Core Technologies
- **Language**: Kotlin 1.8+
- **UI Framework**: Jetpack Compose
- **Architecture**: MVVM (Model-View-ViewModel)
- **Build System**: Gradle with Kotlin DSL

### Libraries & Dependencies
- **AndroidX**: Core, Lifecycle, Activity, Navigation
- **Material 3**: Modern UI components
- **Biometric**: Device authentication
- **Firebase**: Analytics and Firestore
- **Lottie**: Vector animations
- **Kotlin Serialization**: JSON handling

### Development Tools
- **Android Studio**: IDE
- **Firebase Console**: Analytics dashboard
- **Git**: Version control

## 🤝 Contributing

We welcome contributions! This project is part of an academic thesis and contributions help improve device security analysis.

### How to Contribute

1. **Fork the repository**
2. **Create a feature branch**
   ```bash
   git checkout -b feature/your-feature-name
   ```
3. **Make your changes**
4. **Test thoroughly** on multiple Android versions
5. **Commit your changes**
   ```bash
   git commit -m "Add: Brief description of changes"
   ```
6. **Push to your branch**
   ```bash
   git push origin feature/your-feature-name
   ```
7. **Create a Pull Request**

### Development Guidelines
- Follow Kotlin coding standards
- Use meaningful commit messages
- Test on devices with API 24+
- Maintain Material 3 design consistency
- Document new features in code comments

## 👥 Credits

This application was developed as part of a Thesis Project by:

### Development Team
- **Nafiz Ahmed Rhythm** - Main Lead
- **MD Rezaul Karim** - Team Member
- **MD. Shamsul Haque Sakin** - Team Member
- **Fatema Tuz Zohora Panna** - Team Member
- **Asif Imtiaz Chowdhury** - Team Member

### Acknowledgments
- Special thanks to academic advisors and contributors
- Built for enhancing Android device security


---

**Note**: This is an academic project developed for research purposes. While designed for security analysis, always follow best practices for Android development and user privacy.
