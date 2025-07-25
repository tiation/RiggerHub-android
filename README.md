# RiggerHub Android

🏗️ **A ChaseWhiteRabbit NGO Initiative**

## 📍 Repository Location \u0026 Structure\n\n**Current Location**: `/Users/tiaastor/Github/tiation-repos/RiggerHub-android/`\n\nThis repository is part of the **Tiation Enterprise Repository Structure**, specifically designed to house **ChaseWhiteRabbit NGO's** technology initiatives following enterprise-grade development practices.\n\n### 🏗️ Enterprise Ecosystem\n- **Repository Collection**: [Enterprise Repository Index](../ENTERPRISE_REPOSITORY_INDEX.md)\n- **Web Platform**: [RiggerHub-web](../RiggerHub-web/)\n- **Connect Platform**: [RiggerConnect-android](../RiggerConnect-android/), [RiggerConnect-ios](../RiggerConnect-ios/), [RiggerConnect-web](../RiggerConnect-web/)\n- **Backend Services**: [RiggerBackend](../RiggerBackend/)\n- **Shared Libraries**: [RiggerShared](../RiggerShared/)\n\n### 🌟 NGO Integration\nAs a **ChaseWhiteRabbit NGO Initiative**, this project adheres to:\n- ✅ **Enterprise-grade development practices**\n- ✅ **Ethical technology standards**\n- ✅ **Worker empowerment focus**\n- ✅ **DevOps best practices with CI/CD**\n- ✅ **Open development transparency**\n\n## 🎯 Application Overview\n\nRiggerHub Android is an enterprise-grade mobile application serving as the central hub for operations management and coordination among rigger professionals in the construction, oil & gas, and industrial sectors. It provides managers and workers with powerful features for efficient project management and collaboration.

## 🎯 Project Purpose

As part of ChaseWhiteRabbit NGO's mission to enhance 4;ngineering operations, RiggerHub Android offers comprehensive tools to:

- **Manage** large-scale projects and team collaborations
- **Coordinate** resources and personnel for complex tasks
- **Monitor** compliance with modern standards and safety protocols
- **Streamline** communication channels for team-wide updates

## 🔗 Related Repositories

### Core Platform Components

| Repository | Platform | Description | GitHub SSH URL |
|------------|----------|-------------|----------------|
| **RiggerConnect-web** | Web | Business-focused recruitment platform | `git@github.com:tiation/RiggerConnect-web.git` |
| **RiggerConnect-android** | Android | Mobile business management app | `git@github.com:tiation/RiggerConnect-android.git` |
| **RiggerConnect-ios** | iOS | Mobile business management app | `git@github.com:tiation/RiggerConnect-ios.git` |
| **RiggerConnect-capacitor** | Cross-platform | Cross-platform mobile framework | `git@github.com:tiation/RiggerConnect-capacitor.git` |
| **RiggerHub-web** | Web | Worker-focused job search platform | `git@github.com:tiation/RiggerHub-web.git` |
| **RiggerHub-android** | Android | Mobile worker app | `git@github.com:tiation/RiggerHub-android.git` |
| **RiggerHub-ios** | iOS | Mobile worker app | `git@github.com:tiation/RiggerHub-ios.git` |
| **RiggerBackend** | API/Backend | Core backend services and APIs | `git@github.com:tiation/RiggerBackend.git` |
| **RiggerShared** | Multi-platform | Shared libraries and components | `git@github.com:tiation/RiggerShared.git` |

### Enterprise Integration Architecture

```mermaid
graph TB
    RB[RiggerBackend<br/>Core API Services] --> RCW[RiggerConnect-web]
    RB --> RCA[RiggerConnect-android]
    RB --> RCI[RiggerConnect-ios]
    RB --> RHW[RiggerHub-web]
    RB --> RHA[RiggerHub-android]
    RB --> RHI[RiggerHub-ios]
    RS[RiggerShared<br/>Common Libraries] --> RCW
    RS --> RCA
    RS --> RCI
    RS --> RHW
    RS --> RHA
    RS --> RHI
    
    style RHA fill:#00FFFF,color:#000
    style RB fill:#FF00FF,color:#000
    style RS fill:#00FF00,color:#000
```

### ChaseWhiteRabbit NGO License Framework

All repositories in the Rigger ecosystem are licensed under **GPL v3**, ensuring:
- ✅ **Open Source Transparency**: Complete code visibility and community auditing
- ✅ **Ethical Technology Standards**: Algorithmic fairness and bias prevention
- ✅ **Worker Empowerment Focus**: Technology serving users, not corporate profits
- ✅ **Community Ownership**: Improvements benefit the entire rigger community
- ✅ **Corporate Responsibility**: Commercial use must remain open and accessible

## 🚀 Technology Stack

- **Language**: Kotlin 1.9.20
- **Architecture**: MVVM
- **UI Framework**: Jetpack Compose
- **Minimum Android Version**: API 24 (Android 7.0)
- **Target Android Version**: API 34 (Android 14)

## Project Structure

## Project Structure

```
├── .github/workflows/    # CI/CD pipelines
├── configs/             # Configuration files
├── docs/               # Documentation
│   ├── api/           # API documentation
│   ├── architecture/  # System architecture docs
│   ├── deployment/    # Deployment guides
│   └── development/   # Development guides
├── scripts/           # Build and deployment scripts
├── src/              # Source code
└── tests/            # Test suites
```

## Features

- Native Android hub application
- Ethical, enterprise-grade development practices
- DevOps best practices integration
- Modern, striking UI/UX design
- CI/CD ready architecture

## Quick Start

1. Clone the repository
2. Open in Android Studio
3. Configure build variants
4. Run on device/emulator

## Contributing

Please follow our enterprise development standards and ensure all code meets our ethical guidelines.

## 🤝 Project Team & Purpose

This project is part of a broader suite of repositories aimed at supporting the **transient rigging and heavy lifting industry** in Western Australia and beyond.

🔗 **Related Repositories**:

* [`RiggerConnect-web`](https://github.com/ChaseWhiteRabbit/RiggerConnect-web) - Professional networking platform for construction workers
* [`RiggerConnect-android`](https://github.com/ChaseWhiteRabbit/RiggerConnect-android) - Native Android mobile networking application
* [`RiggerConnect-ios`](https://github.com/ChaseWhiteRabbit/RiggerConnect-ios) - Native iOS mobile networking application
* [`RiggerConnect-capacitor`](https://github.com/ChaseWhiteRabbit/RiggerConnect-capacitor) - Cross-platform mobile app built with Ionic Capacitor
* [`RiggerHub-web`](https://github.com/ChaseWhiteRabbit/RiggerHub-web) - Operations management hub for business users
* [`RiggerHub-android`](https://github.com/ChaseWhiteRabbit/RiggerHub-android) - Native Android operations management application
* [`RiggerHub-ios`](https://github.com/ChaseWhiteRabbit/RiggerHub-ios) - Native iOS operations management application
* [`RiggerShared`](https://github.com/ChaseWhiteRabbit/RiggerShared) - Shared libraries, components, and utilities
* [`RiggerBackend`](https://github.com/ChaseWhiteRabbit/RiggerBackend) - Core backend services and APIs for the Rigger ecosystem

📬 **Contact**:
For questions, ideas, or collaboration inquiries, please reach out to:

* **Jack Jonas** – [jackjonas95@gmail.com](mailto:jackjonas95@gmail.com)
* **Tia** – [tiatheone@protonmail.com](mailto:tiatheone@protonmail.com)

---

### 🙌 About the Founders

**Jack Jonas** is a seasoned rigger, crane operator, and heavy vehicle mechanic based in Karratha, Western Australia. His firsthand experience in the field shapes the practical backbone of this platform.

**Tia** is a Swedish software developer and founder of the NGO **ChaseWhiteRabbit**, which is dedicated to building inclusive, systemic solutions to complex challenges.

Together, they created this SaaS platform to:

* Help connect riggers, doggers, and crane operators to real work opportunities.
* Support better logistics, transparency, and compliance in the field.
* Fund and sustain the good work being done by **ChaseWhiteRabbit** in disadvantaged communities.

## 👥 Contact & Team

### Project Leaders

**Jack Jonas** - Karratha Crane Operator & Industry Expert  
📧 [jackjonas95@gmail.com](mailto:jackjonas95@gmail.com)  
🏗️ **Industry Expertise**: Seasoned rigger, crane operator, and heavy vehicle mechanic based in Karratha, Western Australia. Jack's firsthand experience in the field ensures this Android operations management application meets the practical needs of riggers who require mobile tools for coordinating complex projects and managing teams in challenging industrial environments.

**Tia** - ChaseWhiteRabbit NGO Technical Leadership  
📧 [tiatheone@protonmail.com](mailto:tiatheone@protonmail.com)  
🌟 **NGO Mission-Driven Leadership**: Swedish software developer and founder of ChaseWhiteRabbit NGO, dedicated to enhancing engineering operations through ethical technology solutions. Tia's mission-driven approach ensures this platform empowers rigger professionals with robust analytics and performance monitoring tools while maintaining focus on worker welfare and community impact.

### Primary Maintainers

For inquiries related to the Rigger ecosystem, please contact our primary maintainers:

- **Jack Jonas**: [jackjonas95@gmail.com](mailto:jackjonas95@gmail.com)
- **Tia Astor**: [tiatheone@protonmail.com](mailto:tiatheone@protonmail.com)

These maintainers oversee the development and coordination of the entire Rigger platform ecosystem, including RiggerConnect, RiggerHub, RiggerBackend, and RiggerShared repositories.

## License

Enterprise license - Contact ChaseWhiteRabbit NGO for usage rights.

## 🌟 Project Vision: Empowering Industry Through Ethical Technology

### How This Platform Serves Jack Jonas and the Rigging Industry

RiggerHub Android delivers comprehensive mobile operations management specifically designed for the dynamic environment of Western Australia's rigging industry. For professionals like Jack Jonas managing complex projects, this native Android application provides:

- **Mobile-First Operations Management**: Purpose-built Android app optimized for on-site project coordination and team management in challenging industrial environments
- **Real-Time Project Coordination**: Advanced mobile tools for coordinating resources, personnel, and equipment across multiple rigging operations simultaneously
- **Compliance and Safety Management**: Digital oversight of safety protocols, certification tracking, and regulatory compliance requirements specific to rigging operations
- **Team Communication Hub**: Streamlined communication channels enabling effective coordination between project managers, riggers, and support teams
- **Analytics and Performance Monitoring**: Comprehensive project analytics and performance tracking tools that help optimize operations and identify improvement opportunities

### Supporting ChaseWhiteRabbit NGO's Charitable Mission

Every successful project managed through RiggerHub Android generates sustainable funding for ChaseWhiteRabbit NGO's charitable initiatives:

- **Operations Management Impact**: Revenue from mobile operations management features directly supports NGO programs focused on workforce development and community empowerment
- **Project Success Funding**: Platform effectiveness in project coordination enables NGO investment in vocational training programs for disadvantaged youth
- **Mobile Technology Access**: Android app revenue helps establish mobile technology training centers in remote industrial communities
- **Research and Development**: Platform growth supports NGO development of additional open-source tools that benefit operations management in blue-collar industries
- **Industry Standards Advocacy**: Revenue funds research and policy development for improved safety standards and worker protection in industrial operations

### Ethical, Accessible, and Worker-First Technology

RiggerHub Android exemplifies ChaseWhiteRabbit NGO's commitment to technology that enhances operations while empowering workers:

**🔍 Ethical by Design**
- GPL v3 licensing ensures complete transparency and prevents proprietary exploitation of operational data
- Algorithmic fairness in resource allocation and task assignment prevents discrimination and promotes equal opportunity
- Privacy-first architecture with secure local data storage protects sensitive project information
- Anti-bias safeguards in performance analytics ensure fair evaluation regardless of worker background

**♿ Accessibility as a Core Value**
- Material Design compliance with accessibility features for users with diverse abilities
- Multi-language support reflecting the diverse workforce communities in WA's industrial sectors
- Offline-first architecture acknowledging connectivity challenges in remote project sites
- Voice commands and hands-free operation for use in active work environments

**👷 Worker-Focused Philosophy**
- User and project data ownership prevents vendor lock-in and ensures operational continuity
- Transparent analytics that don't exploit workers or compromise their professional standing
- Direct feedback mechanisms giving operations teams genuine voice in platform development
- Performance recognition that values practical experience, safety record, and collaborative skills

This native Android operations platform demonstrates that enterprise-grade mobile technology can simultaneously serve project efficiency needs, empower individual workers, and generate sustainable funding for social good - proving that ethical technology practices create stronger operational outcomes and more sustainable business models.
