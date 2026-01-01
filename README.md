# Mendix-Gamification-Module
A plug-and-play Gamification engine for Mendix apps. Features include XP calculation, automated leveling, and a badge system with a non-intrusive 1-1 User architecture.

A lightweight, scalable Gamification module for Mendix. This module allows developers to quickly integrate user engagement features like **Experience Points (XP)**, **Leveling**, and **Achievements/Badges** without modifying their existing User entities.

## 🚀 Key Features
- **Flexible XP Engine:** Logic to handle XP gains and multi-level jumps.
- **Level Configuration:** Fully data-driven level requirements (Levels 1-50 included).
- **Badge System:** Many-to-Many association architecture for badges and rewards.
- **Ready-to-use UI:** Includes snippets for Profile Cards and Leaderboards.
- **Easy Integration:** Uses a 1-1 association with `System.User` to avoid entity inheritance conflicts.



## 🛠 Installation
1. Download the `.mpk` file.
2. Import the module into your Mendix Project.
3. Map the module security roles (`User` and `Administrator`) to your project roles.
4. Add the `ASu_InitializeLevelConfig` microflow to your app's **After Startup** event.

## 📖 Usage
To reward a user with XP, simply call the `SUB_AddXP` microflow in your logic:
- **User:** The user receiving points.
- **Amount:** The number of points to add.
- **Reason:** A string describing the action (e.g., "Daily Login").



## 🤝 Contributing
Contributions, issues, and feature requests are welcome! Feel free to check the [issues page](https://github.com/alsharefee/Mendix-Gamification-Module/issues).

## 📄 License
This project is [Apache 2.0](LICENSE) licensed.
