# Progressive

![Progressive Logo](https://github.com/h8moss/progressive/raw/main/src-tauri/icons/128x128.png)

A simple, open-source TODO list and progress tracker for Windows and Linux. Built with ❤️ using Tauri and Svelte.

[![License: GPL v3](https://img.shields.io/badge/License-GPLv3-blue.svg)](https://www.gnu.org/licenses/gpl-3.0)
[![GitHub stars](https://img.shields.io/github/stars/h8moss/progressive.svg)](https://github.com/h8moss/progressive/stargazers)
[![GitHub issues](https://img.shields.io/github/issues/h8moss/progressive.svg)](https://github.com/h8moss/progressive/issues)

## 📋 Table of Contents
- [Features](#-features)
- [Getting Started](#-getting-started)
- [Installation](#-installation)
- [Usage](#%EF%B8%8F-usage)
- [Contributing](#-contributing)
- [Roadmap](#%EF%B8%8F-roadmap)
- [Frequently Asked Questions](#-frequently-asked-questions)
- [License](#-license)
- [Acknowledgements](#-acknowledgements)

## 🌟 Features

### 📊 Nested and slider tasks
Organize your work with hierarchical task structures. Break down complex projects into manageable subtasks and keep exact progress on each of them.
![Nested and slider tasks demo](https://raw.githubusercontent.com/h8moss/progressive/refs/heads/main/screenshots/screenshot1.png)

### ⚖️ Task Weights
Assign importance to your tasks. Heavier tasks contribute more to your overall progress.
![Task weights demo](https://github.com/user-attachments/assets/35c0c870-9e79-4ce3-ab2e-be5d9f3fafb5)

### 🔢 Weight Interpretation
Weights can be interpreted and rendered as different units, making it easier to understand task importance in various contexts.

### 🎨 Custom Themes
Personalize your experience with custom color schemes.

## 🚀 Getting Started

### System Requirements
- 2 GB RAM 
- 100 MB free disk space

## 📥 Installation

### Windows
1. Visit the [Releases page](https://github.com/h8moss/progressive/releases) on GitHub.
2. Download the latest version of the application.
3. Run the installer and follow the prompts.

### Linux
Install the app from [its flathub page](https://flathub.org/en/apps/io.github.h8moss.progressive)

### Building from source (Windows, Linux and MacOS)
> [!WARNING]
> The application has not been tested in MacOS, it may or may not work correctly.

1. Install dependencies
    Check tauri's [prerequisites](https://tauri.app/start/prerequisites/) and follow the instructions. You will need to install NodeJS, Rust, and a few other platform-dependent dependencies.

2. Clone the repository:
   ```bash
   git clone https://github.com/h8moss/progressive
   cd progressive
   ```

3. Install dependencies:
   ```bash
   npm install
   ```

4. Build the project:
   ```bash
   npm run tauri build
   ```

If you encounter any issues during installation or have suggestions for improving cross-platform support, please open an issue on our [GitHub repository](https://github.com/h8moss/progressive/issues).
## 🖱️ Usage

1. Launch Progressive from your applications menu or desktop shortcut.
2. Here you may start a new tracker or open an existing one
3. To add new tasks right click anywhere within the main task and click "new child" or press the big plus button at the bottom.
4. To create subtasks first right click any existing task and click "make childful", then right click it and click "new child"

## 🛠️ Customization

### Creating Custom Themes

1. Navigate to `AppData/Roaming/com.h8m0ss.progressive/themes`.
2. Create a new JSON file for each theme.
3. Define the theme properties:

```json
{
  "name": "My Custom Theme",
  "textColor": "#000000",
  "textColorB": "#FFFFFF",
  "backgroundColor": "#F0F0F0",
  "darkenColor": [10, 10, 10],
  "highlightColorA": "#4CAF50",
  "highlightColorB": "#45a049"
}
```

For more details, check out the [default themes](https://github.com/h8moss/progressive/blob/main/src/lib/ProgressNode/constants.ts).

## 🤝 Contributing

We welcome contributions! Here's how you can help:

1. Fork the repository.
2. Create a new branch: `git checkout -b feature/your-feature-name`.
3. Make your changes and commit them: `git commit -m 'Add some feature'`.
4. Push to the branch: `git push origin feature/your-feature-name`.
5. Submit a pull request.

## 🗺️ Roadmap

- [ ] Custom weight units
- [ ] Setting default theme
- [ ] Duplicating tasks

## ❓ Frequently Asked Questions

**Q: Can I sync my tasks across multiple devices?**
A: Progressive is, and will always remain, a fully offline application, we will never send your tasks over to a server, that being said, you can use an application like [syncthing](https://syncthing.net/) to keep your files perpetually synced across devices

**Q: Is there a mobile version available?**
A: Absolutely no!!!! This is something that we do not have planned as it would require a full rewrite of the application

**Q: How can I report a bug or request a feature?**
A: Please use our [GitHub Issues](https://github.com/h8moss/progressive/issues) page to report bugs or suggest new features.

## 📄 License

This project is licensed under the GNU GPLv3 License - see the [LICENSE](LICENSE) file for details.

## 🙏 Acknowledgements

### Icons
- Arrow-right icon by [ByPeople](https://www.bypeople.com?ref=svgrepo.com) (Public Domain)
- Settings icon by [Vmware](https://github.com/vmware/clarity-assets?ref=svgrepo.com) (MIT License)
- Edit and Save icon by [Konstantin Filatov](https://www.figma.com/@thinkcly?ref=svgrepo.com) (CC Attribution License)

Icons sourced from [SVG Repo](https://www.svgrepo.com).

### Technologies
- [Tauri](https://tauri.app/)
- [Svelte](https://svelte.dev/)

---

Made with ☕ by Daniel Armenta © 2023
