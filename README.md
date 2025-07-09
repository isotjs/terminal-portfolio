# 🖥️ Terminal Portfolio - İsot

An interactive terminal-style portfolio website that simulates a real command-line interface. Built with vanilla HTML, CSS, and JavaScript.

![Terminal Portfolio Preview](https://img.shields.io/badge/Status-Active-brightgreen)
![License](https://img.shields.io/badge/License-GPL--3.0-blue)
![Made with](https://img.shields.io/badge/Made%20with-HTML%20%7C%20CSS%20%7C%20JavaScript-orange)

## ✨ Features

- **Interactive Terminal Interface**: Realistic command-line experience
- **AI-Style Responses**: Animated sudo command responses with AI personality
- **Command History**: Navigate through previous commands with arrow keys
- **Auto-completion**: Tab key for command suggestions
- **File System Simulation**: Browse through virtual files and directories
- **Responsive Design**: Works on desktop and mobile devices
- **Theme Support**: Multiple color themes (dark, light, solarized)
- **Real-time Weather**: Simulated weather information
- **System Information**: neofetch-style system display

## 🚀 Live Demo

Visit the live demo: [Terminal Portfolio](https://isotjs.github.io/terminal-portfolio/)

## 🛠️ Technologies Used

- **HTML5**: Structure and semantic markup
- **CSS3**: Styling, animations, and responsive design
- **JavaScript (ES6+)**: Interactive functionality and command processing
- **JetBrains Mono**: Terminal-style font
- **GitHub Pages**: Hosting

## 📋 Available Commands

### Portfolio Commands
- `about` - Display personal information
- `skills` - Show technical skills with progress bars
- `projects` - List featured projects
- `education` - Display educational background
- `contact` - Show contact information

### System Commands
- `help` - Show available commands
- `clear` - Clear terminal screen
- `ls` - List directory contents
- `cat [file]` - Display file contents
- `pwd` - Print working directory
- `cd [dir]` - Change directory
- `whoami` - Display current user
- `date` - Show current date and time
- `neofetch` - Display system information
- `tree` - Show directory tree
- `history` - Show command history
- `echo [text]` - Echo text to terminal

### Interactive Commands
- `sudo [command]` - Try admin commands (with AI responses!)
- `theme [name]` - Change color theme
- `repo` - View source code
- `weather` - Check current weather

## 🎮 Special Features

### AI-Style Sudo Responses
The `sudo` command features animated responses that simulate an AI system:
- Multiple random response messages
- Special easter eggs for different commands
- Animated security protocols
- AI personality responses

### File System Simulation
- Virtual file system with realistic structure
- Browse through projects and documents
- `cat` command to read file contents
- Directory navigation with `cd` and `ls`

## 🎨 Themes

The terminal supports multiple color themes:
- **Dark** (default) - Classic terminal look
- **Light** - Bright theme for daytime use
- **Solarized** - Eye-friendly color scheme

## 📁 Project Structure

```
terminal-portfolio/
├── index.html          # Main HTML file
├── README.md           # This file
└── LICENSE             # GPL-3.0 License
```

## 🚀 Getting Started

### Prerequisites
- A modern web browser (Chrome, Firefox, Safari, Edge)
- No additional dependencies required

### Installation

1. Clone the repository:
```bash
git clone https://github.com/isotjs/terminal-portfolio.git
cd terminal-portfolio
```

2. Open `index.html` in your web browser:
```bash
# On macOS/Linux
open index.html

# On Windows
start index.html
```

Or simply double-click the `index.html` file.

### Development

To modify the portfolio:

1. Edit `index.html` to update content
2. Customize the CSS styles in the `<style>` section
3. Modify JavaScript functions in the `<script>` section
4. Test changes by refreshing the browser

## 🎯 Customization

### Adding New Commands

1. Add the command to the `commands` object in the JavaScript
2. Create the corresponding function
3. Add the command to the help menu

Example:
```javascript
this.commands = {
    // ... existing commands
    mycommand: this.myCommand.bind(this)
};

myCommand(args) {
    this.addOutput(`<span class="info">My custom command!</span>`);
}
```

### Updating Personal Information

Edit the following functions in the JavaScript:
- `showAbout()` - Personal information
- `showSkills()` - Technical skills
- `showProjects()` - Project portfolio
- `showEducation()` - Educational background
- `showContact()` - Contact information

### Modifying the File System

Update the `fileSystem` object to change the virtual file structure:
```javascript
this.fileSystem = {
    '~': {
        type: 'directory',
        contents: {
            'myfile.txt': { type: 'file', content: 'File content here' },
            'mydir': { type: 'directory', contents: {} }
        }
    }
};
```

## 🤝 Contributing

Contributions are welcome! Please feel free to submit a Pull Request.

1. Fork the repository
2. Create your feature branch (`git checkout -b feature/AmazingFeature`)
3. Commit your changes (`git commit -m 'Add some AmazingFeature'`)
4. Push to the branch (`git push origin feature/AmazingFeature`)
5. Open a Pull Request

## 📝 License

This project is licensed under the GNU General Public License v3.0 - see the [LICENSE](LICENSE) file for details.

## 🙏 Acknowledgments

- Inspired by terminal interfaces and command-line tools
- Font: [JetBrains Mono](https://www.jetbrains.com/lp/mono/)
- Icons: Unicode emojis and symbols
- Design: Modern terminal aesthetic

## 📊 Project Status

- ✅ Core functionality complete
- ✅ Responsive design implemented
- ✅ AI-style interactions added
- ✅ File system simulation working
- ✅ Multiple themes available
- 🔄 Continuous improvements

---

⭐ If you find this project useful, please give it a star :)
