# Trivia Quiz Game 🎯

Welcome to **Trivia Quiz Game**, an engaging and interactive quiz application that tests your knowledge across various topics. This script is designed to run seamlessly on both GUI and CLI environments, making it perfect for desktop Linux systems, servers, and Termux users alike.

## ✨ Features

### Core Gameplay
- **25 Comprehensive Questions** covering geography, science, history, technology, and more
- **Smart Progress Tracking** - automatically saves after each question
- **Resume Functionality** - continue where you left off or start fresh
- **Detailed Statistics** - tracks correct answers, wrong answers, and percentage score
- **Tiered Performance Feedback** - get personalized feedback based on your score

### Dual Interface Support
- **🖥️ GUI Mode** - Beautiful Zenity-based dialogs for graphical environments
- **⌨️ CLI Mode** - Colorful terminal interface with full ANSI color support
- **🔄 Auto-Detection** - Automatically selects the best mode for your environment
- **🎨 Rich Visual Experience** - Colors, emojis, and clean formatting in both modes

### Smart Features
- **Auto-Update System** - checks for new versions and prompts for updates
- **Safe Exit Anytime** - press Cancel (GUI) or 'q' (CLI) to exit with progress saved
- **Cross-Platform Compatible** - works on any Linux distribution, Termux, and more
- **Lightweight & Fast** - minimal dependencies, quick startup

## 🚀 Getting Started

### Quick Start

Clone the repository and run the script:

```bash
# Clone the repository
git clone https://github.com/uzairdeveloper223/trivia-with-zenity.git

# Navigate to the directory
cd trivia-with-zenity

# Make the script executable
chmod +x quiz

# Run the script (auto-detects mode)
bash quiz
```

### Usage Options

```bash
# Auto-detect mode (GUI if available, otherwise CLI)
bash quiz

# Force CLI mode (perfect for Termux, SSH, or servers)
bash quiz --cli

# Force GUI mode (requires Zenity and DISPLAY)
bash quiz --gui
```

## 📋 Requirements

### For GUI Mode
- **Linux with GUI** - Any Linux distribution with graphical environment
- **Termux with Xfce/VNC** - Termux users need a desktop environment setup
- **Zenity** - Install using: `apt-get install zenity` or `pkg install zenity`
- **DISPLAY variable** - Must be set for X11/Wayland

### For CLI Mode
- **Any Linux/Unix System** - Works on servers, containers, WSL
- **Termux** - Full support without GUI setup
- **Bash Shell** - Version 4.0 or higher recommended
- **Terminal with color support** - For best visual experience

### Optional Dependencies
- **curl** - For automatic updates (usually pre-installed)

## 🎮 How to Play

### GUI Mode
1. Launch the quiz and you'll see dialog boxes with questions
2. Select your answer from the radio buttons
3. Get instant feedback with emoji-rich messages
4. Press Cancel anytime to save and exit
5. View your final score with performance tier

### CLI Mode
1. Start the quiz to see colorful terminal interface
2. Type the number (1-4) corresponding to your answer
3. Press 'q' anytime to save progress and exit
4. See real-time score updates after each question
5. Get detailed statistics at the end

## 📊 Scoring System

Your performance is rated based on correct answers:

| Score Range | Rating | Description |
|-------------|--------|-------------|
| 25/25 | 🏆 Perfect Score | You're a trivia master! |
| 20-24 | 🌟 Excellent | Outstanding performance! |
| 15-19 | 👏 Great Job | You did well! |
| 10-14 | 😊 Good Effort | Keep practicing! |
| 0-9 | 📚 Keep Learning | Practice makes perfect! |

## 🔧 Features in Detail

### Auto-Save System
- Progress automatically saves after every question
- Resume anytime without losing your score
- Safe exit mechanism prevents data loss
- Option to restart fresh on each launch

### Update Manager
- Checks for new versions on startup
- One-click update from GitHub repository
- Preserves your current progress during updates
- Version tracking and changelog support

### Cross-Platform Support
```bash
# Works perfectly on:
✅ Ubuntu/Debian Desktop
✅ Fedora/RHEL/CentOS
✅ Arch Linux
✅ Termux (Android)
✅ WSL (Windows Subsystem for Linux)
✅ SSH Sessions
✅ Docker Containers
✅ Raspberry Pi
```

## 🎨 Screenshots

### GUI Mode
Beautiful Zenity dialogs with question display, radio button options, and instant feedback messages.

### CLI Mode
Colorful terminal interface with:
- Cyan headers and banners
- Green for correct answers
- Red for wrong answers
- Yellow for prompts
- Real-time progress tracking

## 🛠️ Configuration

### Data Storage
- Quiz data is stored in `./Quiz-data/data.txt`
- Contains: score, current question, correct/wrong answers
- Automatically created on first run

### Customization
Edit the script to:
- Add more questions to the `questions` array
- Change color schemes (CLI mode)
- Modify dialog dimensions (GUI mode)
- Adjust timeout durations

## 🐛 Troubleshooting

### Zenity not found (GUI mode)
```bash
# Debian/Ubuntu
sudo apt-get update && sudo apt-get install zenity -y

# Termux
pkg install zenity -y

# Fedora/RHEL
sudo dnf install zenity -y
```

### DISPLAY not set
```bash
# Set DISPLAY variable (Termux with VNC)
export DISPLAY=:1

# Or force CLI mode
bash quiz --cli
```

### Permission denied
```bash
# Make script executable
chmod +x quiz
```

### Colors not showing (CLI mode)
- Ensure your terminal supports ANSI colors
- Try a different terminal emulator
- Check if `TERM` variable is set correctly

## 🔄 Future Updates

Planned features and improvements:

- [ ] **More Questions** - Expanding to 50+ questions
- [ ] **Difficulty Levels** - Easy, Medium, Hard modes
- [ ] **Categories** - Science, History, Geography, Tech, etc.
- [ ] **Multiplayer Support** - Compete with friends
- [ ] **Leaderboard System** - Track high scores
- [ ] **Custom Quiz Creator** - Add your own questions
- [ ] **Time Challenge Mode** - Race against the clock
- [ ] **Achievement System** - Unlock badges and rewards
- [ ] **Multi-language Support** - Translations for global users
- [ ] **Sound Effects** - Audio feedback (GUI mode)

Stay tuned for regular updates with new questions, improved functionality, and exciting features!

## 📜 License

This project is licensed under the MIT License. See the [LICENSE](./LICENSE) file for more details.

## 🤝 Contributing

Contributions are welcome! Here's how you can help:

### Ways to Contribute
- 🐛 Report bugs and issues
- 💡 Suggest new features or questions
- 📝 Improve documentation
- 🔧 Submit pull requests with enhancements
- ⭐ Star the repository if you find it useful

### Contribution Guidelines
1. Fork the repository
2. Create a feature branch (`git checkout -b feature/AmazingFeature`)
3. Commit your changes (`git commit -m 'Add some AmazingFeature'`)
4. Push to the branch (`git push origin feature/AmazingFeature`)
5. Open a Pull Request

### Adding Questions
To add new questions, edit the `questions` array in the script:
```bash
"Your question here?|Option1|Option2|Option3|Option4|CorrectAnswer"
```

## 📞 Contact & Support

- **Developer**: Uzair Mughal (uzairdeveloper223)
- **Email**: contact@uzair.is-a.dev
- **Website**: [uzair.is-a.dev](https://uzair.is-a.dev)
- **GitHub**: [@uzairdeveloper223](https://github.com/uzairdeveloper223)

### Get Help
- 📖 Check the [Wiki](https://github.com/uzairdeveloper223/trivia-with-zenity/wiki) for detailed guides
- 🐛 [Report Issues](https://github.com/uzairdeveloper223/trivia-with-zenity/issues) on GitHub
- 💬 [Discussions](https://github.com/uzairdeveloper223/trivia-with-zenity/discussions) for questions

## 🌟 Acknowledgments

- Built with ❤️ by **Uzairdeveloper223**
- Powered by **Bash**, **Zenity**, and **ANSI Colors**
- Thanks to all contributors and users!
- Special thanks to the open-source community

## 📈 Version History

### v2.0 (Current)
- ✨ Added CLI mode support
- 🎨 Colorful terminal interface
- 🔄 Auto-mode detection
- 💾 Enhanced progress saving
- 📊 Percentage scoring system
- 🎯 Performance tier ratings
- 🔧 Code refactoring and optimization
- 🐛 Bug fixes and improvements

### v1.0
- 🎉 Initial release
- 🖥️ GUI mode with Zenity
- 📝 10 quiz questions
- 💾 Basic progress saving
- 🔄 Update system

---

<div align="center">

**[⬆ Back to Top](#trivia-quiz-game-)**

Made with 💚 by [Uzair Mughal](https://uzair.is-a.dev)

If you found this helpful, consider giving it a ⭐!

</div>
