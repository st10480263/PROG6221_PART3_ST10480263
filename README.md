# CyberBot — Part 3

An optimized, professional-grade interactive WPF security chatbot application designed to demonstrate robust relational database management, asynchronous UI animation threads, and automated system schema compilation.

## 🛠️ Architectural Highlights

* **Data Tier Decoupling (Relational Pipeline):** Data transactions are separated out of the presentation loop. Information is ingested and written directly to a local engine instance backed by a MySQL database storage array.
* **Asynchronous UI Thread Syncing:** Utilizes an active `DispatcherTimer` state machine to manage localized string parsing and render text letter-by-letter, avoiding UI blocking during heavy message queues.
* **Automated Schema Self-Healing:** The system manages its own data tier execution. On boot, it checks connectivity and automatically initializes database configurations and structural tables if they do not exist.
* **Bulletproof Exception Boundaries (Fault-Tolerance):** Outfitted with robust try-catch safety blocks. If the target MySQL engine drops offline, the system intercepts the runtime error and seamlessly routes inputs to a simulation cache array so the app never crashes.

## 📋 Implemented Features

### 1. Relational Task Registration
Users can dynamically initiate a multi-stage goal workflow using the `add task - [Title]` format. The system intercepts the string via parsing rules, transitions into a state listener, captures description details, and commits the record via parameterized `INSERT INTO` commands to prevent SQL Injection exploits.

### 2. Responsive Visual Speech Bubbles
The layout completely drops standard raw text rendering in favor of custom speech bubble border rows. Elements dynamically calculate orientation rows (Right-aligned Cadet Blue for the User, Left-aligned Dark Slate Blue for the Bot) and auto-wrap string contents across varying screen dimensions.

### 3. Integrated 10-Question Evaluation Matrix
Features an interactive 10-question cybersecurity quiz mini-game that evaluates comprehension matrices. The system parses structural true/false layouts and multiple-choice options, tracks scoring arrays, and outputs real-time explanation feedback pulled from Information Security (ISEC) and Systems Analysis and Design (SAND) fundamentals.

### 4. Dependency Restoration Layer
To maintain source control size compliance, all heavy `.dll` database driver binaries and NuGet package folders are excluded from tracking. The architecture features automatic restoration instructions via internal system configurations upon solution re-compilation.

### 5. NuGet Packages
In order to fully utilize the application please reinstate the NuGet MySQL packages for the databases

## 🚀 How to Run the Project

1. Ensure a local instance of **MySQL Server** is running on `localhost:3306` with credentials matching your local class configurations.
2. Open the solution file (`.sln`) inside Visual Studio.
3. Right-click the Solution and select **Restore NuGet Packages** to automatically fetch the database driver libraries.
4. Press **F5** to initialize the interactive security console.

## 🎥 YouTube Explanation Video Outline

A walk-through video explaining the implementation architecture is structured into the following sections:
* **Part 1:** Interactive Demo of the Speech Bubble Interface and Asynchronous Typing Scheduler.
* **Part 2:** Relational Data Tier Walkthrough.
* **Part 3:** Fault-Tolerance Verification.
