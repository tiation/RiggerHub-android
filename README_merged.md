# RiggerHub Android

[![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT)
[![Android Version](https://img.shields.io/badge/Android-8%2B-green)](https://developer.android.com/)
[![Kotlin](https://img.shields.io/badge/Kotlin-1.9%2B-purple)](https://kotlinlang.org/)
[![CI/CD](https://img.shields.io/badge/CI%2FCD-ready-green)](https://gitlab.sxc.codes)

Enterprise-grade Android application for RiggerHub - Construction and mining industry recruitment platform for Western Australia.

## Overview

RiggerHub Android is a cutting-edge mobile application designed for construction and mining professionals in Western Australia. Built with modern Android development practices and following enterprise-grade standards.

## 🎯 Purpose

RiggerHub Android is the comprehensive mobile **worker application** for skilled riggers to discover opportunities, manage profiles, and connect with employers on-the-go. This enterprise-grade native Android application empowers workers with career advancement tools optimized for mobile workflows.

**Key Focus**: Empowering riggers with mobile access to find quality work, showcase skills, manage certifications, and build sustainable careers.

## Features

- User authentication and profile management
- Job search and application functionality
- Real-time notifications
- Compliance tracking
- Safety documentation
- Business networking

## ChaseWhiteRabbit NGO

This project is developed in partnership with ChaseWhiteRabbit NGO, supporting ethical recruitment practices in the construction and mining industry.

RiggerHub Android proudly supports the **ChaseWhiteRabbit NGO** mission of creating positive social impact through technology.

### Our Commitment
- **10% of all profits** are automatically donated to social impact initiatives
- **Partnership Details**: Mobile-first worker empowerment supporting Western Australia's construction, mining, and resources sector
- **Digital Inclusion**: Providing accessible mobile tools for all skill levels
- **Skills Development**: Mobile access to training resources and certification programs
- **Fair Employment**: Supporting ethical work practices through technology

## Development

This repository follows modular, CI/CD-ready development practices.

### Documentation Structure

- `docs/business/` - Business requirements and specifications
- `docs/contracts/` - Contract management documentation
- `docs/safety/` - Safety compliance documentation

## 🚀 Technologies Used

### Core Stack
- **Language**: Kotlin with coroutines
- **Architecture**: MVVM with clean architecture
- **UI Framework**: Jetpack Compose
- **Navigation**: Navigation Component
- **Dependency Injection**: Hilt
- **Networking**: Retrofit with OkHttp
- **Database**: Room with SQLite
- **Image Loading**: Coil
- **Real-time**: WebSocket with OkHttp

### Enterprise Infrastructure
- **Build System**: Gradle with Kotlin DSL
- **CI/CD**: GitLab CI with automated testing and deployment
- **App Distribution**: Google Play Store with staged rollouts
- **Crash Reporting**: Firebase Crashlytics
- **Analytics**: Firebase Analytics with worker-specific events
- **Security**: ProGuard/R8 obfuscation
- **Performance**: App startup optimization and battery efficiency

## 📋 Prerequisites

- Android Studio Arctic Fox or higher
- JDK 11 or higher
- Android SDK 33+
- Kotlin 1.9+

## 🛠️ Setup Instructions

### Development Setup

```bash
# Clone the repository
git clone git@github.com:tiation/RiggerHub-android.git
cd RiggerHub-android

# Open in Android Studio
# File -> Open -> Select project directory

# Sync project with Gradle files
# Build -> Sync Project with Gradle Files

# Run on device/emulator
# Run -> Run 'app'
```

### Build Configuration

```kotlin
android {
    compileSdk 34
    
    defaultConfig {
        applicationId "com.riggerhub.workers"
        minSdk 26
        targetSdk 34
        versionCode 1
        versionName "1.0.0"
    }
    
    buildTypes {
        debug {
            buildConfigField("String", "API_BASE_URL", "\"https://api-dev.rigger.com\"")
            buildConfigField("int", "NGO_DONATION_PERCENTAGE", "10")
            isDebuggable = true
        }
        release {
            buildConfigField("String", "API_BASE_URL", "\"https://api.rigger.com\"")
            buildConfigField("int", "NGO_DONATION_PERCENTAGE", "10")
            isMinifyEnabled = true
            proguardFiles(getDefaultProguardFile("proguard-android-optimize.txt"), "proguard-rules.pro")
        }
    }
}
```

## 🏗️ Architecture Overview

```
app/src/main/java/com/riggerhub/workers/
├── data/               # Data layer (repositories, network, database)
├── domain/             # Business logic (use cases, models)
├── presentation/       # UI layer (composables, viewmodels)
│   ├── auth/          # Authentication screens
│   ├── profile/       # Worker profile management
│   ├── jobs/          # Job discovery and applications
│   ├── bookings/      # Booking management
│   └── certifications/ # Skills and certification management
├── di/                # Dependency injection modules
├── utils/             # Utility classes and extensions
└── MainActivity.kt    # Main entry point
```

## ✨ Key Features

### Professional Profile
- Comprehensive skill and certification management
- Portfolio showcase with project photos
- Digital document storage for certificates
- Professional networking capabilities

### Job Discovery
- Advanced search with location and skill filters
- Real-time job alerts and push notifications
- Swipe-to-apply interface for quick applications
- Saved jobs and application tracking

### Booking Management
- Accept/decline booking requests with one tap
- Calendar integration for scheduling
- Real-time booking status updates
- GPS-enabled check-in for job sites

### Skills & Certifications
- Digital certification wallet
- Skill assessment and verification
- Training resource recommendations
- Compliance tracking and reminders

### Earnings & Analytics
- Payment tracking and history
- Work analytics and performance metrics
- Tax document generation
- Earning forecasts and insights

## 🔄 CI/CD Pipeline

### GitLab CI Configuration

```yaml
stages:
  - test
  - build
  - deploy

android-test:
  stage: test
  image: openjdk:11-jdk
  script:
    - ./gradlew testDebugUnitTest
    - ./gradlew connectedAndroidTest
  coverage: '/Total.*?([0-9]{1,3})%/'

android-build:
  stage: build
  script:
    - ./gradlew assembleRelease
    - ./gradlew bundleRelease
  artifacts:
    paths:
      - app/build/outputs/

play-store-deploy:
  stage: deploy
  script:
    - fastlane deploy
  only:
    - main
```

### Deployment Strategy

- **Internal Testing**: Play Console internal testing with developers
- **Alpha Testing**: Closed testing with select riggers
- **Beta Testing**: Open testing with broader worker community
- **Production**: Staged rollout starting at 5% of users

## 🧪 Testing Strategy

```bash
# Unit tests
./gradlew testDebugUnitTest

# Instrumented tests
./gradlew connectedAndroidTest

# UI tests with Espresso
./gradlew connectedDebugAndroidTest

# Performance testing
./gradlew :benchmark:connectedBenchmarkAndroidTest
```

## 📊 Monitoring & Analytics

- **Worker Analytics**: Job application success rates, earnings tracking
- **Performance**: App startup time, battery usage optimization
- **User Experience**: Feature usage patterns and user flows
- **Business Metrics**: NGO impact tracking and donation transparency

## 🔒 Security & Compliance

- **Biometric Authentication**: Fingerprint and face authentication
- **Certificate Security**: Encrypted storage for professional documents
- **Location Privacy**: Opt-in location sharing with granular controls
- **Payment Security**: PCI DSS compliant payment handling
- **Data Portability**: GDPR compliant data export functionality

## 📞 Support & Contact

- **Technical Issues**: Create an issue in GitLab at `gitlab.sxc.codes`
- **Worker Support**: support@riggerhub.com
- **Business Inquiries**: tiatheone@protonmail.com
- **Security Concerns**: security@riggerhub.com
- **NGO Partnership**: partnerships@chasewhiterabbit.org

## 🔗 Related Repositories

- **RiggerHub-web**: Web version of the worker application
- **RiggerConnect-android**: Android app for businesses
- **RiggerBackend**: Backend services and APIs
- **RiggerShared**: Shared components and utilities

## License

MIT License - Part of the ChaseWhiteRabbit NGO initiative for Western Australia's construction, mining, and resources sector.

Enterprise-grade, ethical development following DevOps best practices.

---

**Built with ❤️ by the Tiation team | Empowering riggers through mobile technology | Supporting social impact through ChaseWhiteRabbit NGO**
