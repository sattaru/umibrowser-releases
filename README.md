# 🐙 UMI Browser - Safe, Friendly, Smart

**UMI = Unstoppable Mindful Intelligence**

A professional, kid-friendly web browser with AI chat, parental controls, and multi-provider AI support. Built with React, Electron, and modern security practices.

*Inspired by Aarush and Adarsh Sattaru.*

---

## ✨ Key Features

### For Kids 👧
- 💬 **UmiChat** - Default AI chat interface powered by multiple providers
- 🔍 **Safe Search** - Curated list of 100+ kid-friendly websites
- 🎤 **Voice Search** - Ask questions using your voice
- 🎨 **Beautiful UI** - Professional, engaging design
- ⏰ **Time Controls** - Browse during parent-approved hours
- 🌐 **Safe Browsing** - Automatic blocking of inappropriate sites

### For Parents 👨‍👩‍👧
- 🔑 **Multi-Provider API** - Support for Google Gemini, Anthropic Claude, Grok, Kimik, OpenAI
- 📋 **Chat History** - Review all Q&A from your kids
- 🆘 **Safety Flags** - Automatic detection of concerning content
- 📊 **Activity Dashboard** - Monitor browsing and chat activity
- ⏱️ **Time Limits** - Set allowed browsing hours
- 🚫 **Content Filtering** - Block categories (adult, gambling, gaming, social media)
- 🔐 **Secure Storage** - API keys stored in system keychain

---

## 🚀 Quick Start

### Installation

Download the installer for your platform from the
**[Latest Release](https://github.com/sattaru/umi/releases/latest)** page. The
direct-download links below always resolve to the newest published build:

#### Windows
- **[UMI Browser EXE (NSIS installer, x64)](https://github.com/sattaru/umi/releases/latest/download/UMI-Browser-win-x64.exe)** - Full installer
- **[UMI Browser MSI (Windows Installer, x64)](https://github.com/sattaru/umi/releases/latest/download/UMI-Browser-win-x64.msi)** - Enterprise-friendly MSI

#### macOS
- **[UMI Browser DMG (Apple Silicon)](https://github.com/sattaru/umi/releases/latest/download/UMI-Browser-mac-arm64.dmg)** - M1/M2/M3
- **[UMI Browser DMG (Intel)](https://github.com/sattaru/umi/releases/latest/download/UMI-Browser-mac-x64.dmg)** - Intel Macs
- **[UMI Browser ZIP (Apple Silicon)](https://github.com/sattaru/umi/releases/latest/download/UMI-Browser-mac-arm64.zip)** - Portable
- **[UMI Browser ZIP (Intel)](https://github.com/sattaru/umi/releases/latest/download/UMI-Browser-mac-x64.zip)** - Portable

#### Linux
- **[UMI Browser AppImage (x64)](https://github.com/sattaru/umi/releases/latest/download/UMI-Browser-linux-x64.AppImage)** - Universal Linux app (no install needed)
- **[UMI Browser DEB (x64)](https://github.com/sattaru/umi/releases/latest/download/UMI-Browser-linux-x64.deb)** - For Ubuntu/Debian

### From Source

```bash
# Clone repository
git clone https://github.com/sattaru/umi.git
cd umi

# Install dependencies
npm install

# Start development
npm run desktop:dev

# Build installers
npm run package:all
```

---

## 📖 Documentation

### Getting Started
- **[Quick Start Guide](./QUICK_START.md)** - Setup in 5 minutes
- **[User Guide](./USER_GUIDE.md)** - Features overview

### For Parents
- **[Parent Setup Guide](./PARENT_SETUP.md)** - Configure controls & API keys
- **[Safety Features](./SAFETY_FEATURES.md)** - Content moderation & alerts

### For Developers
- **[Build & Distribution](./BUILD_AND_DISTRIBUTION.md)** - Package for all platforms
- **[Design System](./DESIGN_AUDIT.md)** - UI/UX specifications
- **[API Integration](./MULTI_PROVIDER_API_GUIDE.md)** - Add AI providers
- **[Features Summary](./FEATURES_SUMMARY.md)** - Complete feature list

---

## 🏗️ Architecture

### Tech Stack
- **Frontend:** React 19 + Vite
- **Desktop:** Electron 31
- **Styling:** CSS3 + Design System tokens
- **APIs:** Multiple AI providers (Gemini, Claude, Grok, etc.)
- **Storage:** System keychain (secure)

### Project Structure
```
umi/
├── src/
│   ├── components/        # React components
│   ├── utils/            # Utilities (API, safety, history)
│   ├── styles/           # CSS (design system)
│   ├── config/           # Configuration
│   └── App.jsx           # Main app
├── electron/             # Electron backend
│   ├── main.cjs          # Main process
│   ├── preload.cjs       # Secure API bridge
│   └── multi-provider-api.cjs
├── BUILD_AND_DISTRIBUTION.md  # Build guide
└── package.json          # Dependencies & scripts
```

---

## 🔐 Security & Privacy

✅ **API Keys** - Never exposed to frontend, stored in system keychain
✅ **Content Moderation** - Automatic detection of harmful content
✅ **Personal Info Protection** - Prevents sharing addresses, passwords, etc.
✅ **Crisis Support** - Self-harm detection with support links
✅ **Offline Mode** - Works without internet connection
✅ **Secure IPC** - Encrypted communication between processes

---

## 🛠️ Build Instructions

### Prerequisites
- Node.js 18+
- npm 10+
- Python 3.6+ (for build tools)

### Build Steps
```bash
# Install dependencies
npm install

# Build web assets
npm run build:web

# Package for your platform
npm run package:win      # Windows (EXE + MSI)
npm run package:mac      # macOS (DMG + ZIP)
npm run package:linux    # Linux (AppImage + DEB)
npm run package:all      # All platforms
```

### Build Configuration
See **[BUILD_AND_DISTRIBUTION.md](./BUILD_AND_DISTRIBUTION.md)** for:
- Icon setup
- Code signing
- Auto-update configuration
- Release checklist

---

## 📋 System Requirements

### Windows
- Windows 7 or later
- 100MB disk space

### macOS
- macOS 10.13 or later
- Intel or Apple Silicon (M1/M2/M3)

### Linux
- Ubuntu 18.04+, Debian 10+, CentOS 7+
- 100MB disk space

---

## 🎯 Getting Started Guides

### For New Users
1. [Quick Start Guide](./QUICK_START.md) - Setup in 5 minutes
2. [Install & Launch](./BUILD_AND_DISTRIBUTION.md#-installation-instructions) - Platform-specific instructions
3. [First Chat](./USER_GUIDE.md) - Start using UmiChat

### For Parents
1. [Parent Setup](./PARENT_SETUP.md) - Configure controls
2. [Add API Keys](./MULTI_PROVIDER_API_GUIDE.md) - Enable AI providers
3. [Monitor Activity](./FEATURES_SUMMARY.md) - Review chat history

### For Developers
1. [Development Setup](./BUILD_AND_DISTRIBUTION.md) - Build from source
2. [Design System](./DESIGN_AUDIT.md) - UI components
3. [API Integration](./MULTI_PROVIDER_API_GUIDE.md) - Add providers
4. [Architecture](./FEATURES_SUMMARY.md) - System design

---

## 📦 Downloads

### Latest Release
- **Version:** 0.0.1
- **Release Date:** April 2026
- **Downloads:** [GitHub Releases](https://github.com/sattaru/umi/releases)

### Installation Links
| Platform | Architecture | Download | Instructions |
|----------|--------------|----------|--------------|
| Windows | x64 | [EXE](https://github.com/sattaru/umi/releases/latest/download/UMI-Browser-win-x64.exe) | Run installer |
| Windows | x64 | [MSI](https://github.com/sattaru/umi/releases/latest/download/UMI-Browser-win-x64.msi) | `msiexec /i UMI-Browser-win-x64.msi` |
| macOS | Apple Silicon | [DMG](https://github.com/sattaru/umi/releases/latest/download/UMI-Browser-mac-arm64.dmg) | Drag to Applications |
| macOS | Intel | [DMG](https://github.com/sattaru/umi/releases/latest/download/UMI-Browser-mac-x64.dmg) | Drag to Applications |
| Linux | x64 | [AppImage](https://github.com/sattaru/umi/releases/latest/download/UMI-Browser-linux-x64.AppImage) | `chmod +x *.AppImage && ./*.AppImage` |
| Ubuntu/Debian | x64 | [DEB](https://github.com/sattaru/umi/releases/latest/download/UMI-Browser-linux-x64.deb) | `sudo dpkg -i UMI-Browser-linux-x64.deb` |

---

## 🚀 Development

### Running Locally
```bash
npm install
npm run desktop:dev
```

### Development Tools
- Hot reload enabled
- DevTools available (F12)
- Console logging for debugging

### Testing
```bash
npm run test              # Run tests
npm run test:ui          # Test UI
npm run test:coverage    # Coverage report
```

---

## 📝 Documentation Index

| Document | Purpose |
|----------|---------|
| [BUILD_AND_DISTRIBUTION.md](./BUILD_AND_DISTRIBUTION.md) | 📦 Complete build & distribution guide |
| [DESIGN_AUDIT.md](./DESIGN_AUDIT.md) | 🎨 Design system specifications |
| [DESIGN_IMPLEMENTATION_GUIDE.md](./DESIGN_IMPLEMENTATION_GUIDE.md) | 🔧 Component integration guide |
| [MULTI_PROVIDER_API_GUIDE.md](./MULTI_PROVIDER_API_GUIDE.md) | 🤖 AI provider setup |
| [FEATURES_SUMMARY.md](./FEATURES_SUMMARY.md) | ✨ Complete feature overview |
| [QUICK_START.md](./QUICK_START.md) | ⚡ 5-minute setup guide |
| [PARENT_SETUP.md](./PARENT_SETUP.md) | 👨‍👩‍👧 Parent configuration guide |
| [USER_GUIDE.md](./USER_GUIDE.md) | 📚 Feature usage guide |

---

## 🤝 Contributing

Contributions welcome! Please:
1. Fork the repository
2. Create feature branch (`git checkout -b feature/amazing`)
3. Commit changes (`git commit -am 'Add amazing feature'`)
4. Push to branch (`git push origin feature/amazing`)
5. Open Pull Request

---

## 📄 License

MIT License - See LICENSE file for details

---

## 🆘 Support

### Getting Help
1. **Documentation:** Check relevant guide above
2. **Issues:** [GitHub Issues](https://github.com/sattaru/umi/issues)
3. **Discussions:** [GitHub Discussions](https://github.com/sattaru/umi/discussions)

### Known Issues
- NTP time validation may fail without internet (uses system time as fallback)
- Some AI providers require valid API keys
- First launch may take 10-15 seconds while assets load

---

## 🎉 Roadmap

### Current (v0.0.1)
- ✅ UmiChat with multiple AI providers
- ✅ Parental controls & monitoring
- ✅ Safety content moderation
- ✅ Professional UI design

### Future (v0.1.0)
- 🔄 Dark mode toggle
- 🔄 Custom themes
- 🔄 Cloud sync backup
- 🔄 Multi-child support
- 🔄 Email parent alerts
- 🔄 Custom safe site list

### Planned (v0.2.0+)
- 📱 Mobile app
- 🎮 Educational games
- 📚 Learning materials
- 🏆 Reward system
- 👥 Family accounts

---

## 👋 About

**UMI Browser** is designed to make the web safer for kids while empowering parents with insights and controls.

**Mission:** Provide a trustworthy, intelligent browsing experience that protects children while respecting their curiosity and independence.

**Inspiration:** Built for Aarush and Adarsh Sattaru, this browser combines security, education, and fun.

---

## 📞 Contact

- **Email:** team@umi-browser.local
- **GitHub:** [UMI Browser](https://github.com/sattaru/umi)
- **Website:** [umi-browser.com](https://umi-browser.com)

---

**🐙 UMI Browser - Making the web safer, one child at a time.**

*Last Updated: April 2026*
