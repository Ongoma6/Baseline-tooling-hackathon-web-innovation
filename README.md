# Baseline-tooling-hackathon-web-innovation
# Baseline Insights - VS Code Extension

🚀 **Winner of the Baseline Tooling Hackathon 2025**

A powerful VS Code extension that provides real-time web feature compatibility insights using Baseline data. Never wonder "Is it safe to use yet?" again!

## ✨ Features

### 🔍 **Real-time Compatibility Analysis**
- **Hover tooltips** showing Baseline status for CSS properties, JavaScript APIs, and HTML elements
- **Visual indicators** with color-coded underlines (✅ green = Baseline, ⚠️ yellow = limited, ❌ red = experimental)
- **Smart autocomplete** that prioritizes Baseline features

### 📊 **Project Overview Dashboard**
- **Sidebar panel** with project-wide compatibility score
- **Current file analysis** showing which features are being used
- **Compatibility reports** with actionable insights

### 🛠️ **Developer-Friendly Tools**
- **Command palette integration** for quick analysis
- **Status bar indicator** showing project health
- **Configurable warnings** with strict mode support

## 🎯 Why Baseline Insights?

Stop jumping between MDN, caniuse.com, and blog posts. Get instant answers about web feature compatibility directly in your editor:

- ✅ **"Is CSS Container Queries safe to use?"** → Hover and see instantly
- ⚠️ **"Should I add a polyfill for this?"** → Get recommendations in tooltips  
- 📊 **"How Baseline-ready is my project?"** → Check the sidebar score

## 🚀 Installation

1. Clone this repository
2. Run `npm install`
3. Press `F5` to launch Extension Development Host
4. Open a CSS, JavaScript, or HTML file
5. Hover over web features to see Baseline status!

## 💡 How It Works

The extension integrates with the [`web-features`](https://github.com/web-platform-dx/web-features) npm package to provide accurate, up-to-date information about web feature support and Baseline status.

### Supported Languages
- **CSS/SCSS/Less**: Grid, Flexbox, Container Queries, Subgrid, and more
- **JavaScript/TypeScript**: Fetch API, Intersection Observer, and modern APIs
- **HTML**: Dialog element, form features, and semantic elements

## 🎨 Screenshots

### Hover Tooltips
Beautiful tooltips showing:
- Baseline status with clear visual indicators
- Browser support matrix
- MDN documentation links
- Usage recommendations

### Sidebar Panel
- Project compatibility overview
- Current file feature analysis
- Quick access to available Baseline features

### Smart Autocomplete
- Baseline features prioritized in suggestions
- Status indicators in completion items
- Helpful documentation preview

## ⚙️ Configuration

```json
{
  "baseline-insights.enableHover": true,
  "baseline-insights.enableDiagnostics": true,
  "baseline-insights.strictMode": false,
  "baseline-insights.targetSupport": "high"
}
```

## 🏆 Built for the Baseline Tooling Hackathon

This extension addresses the core problem developers face: **uncertainty about when web features are safe to use in production**. 

### Innovation Points:
- **Real-time integration** with VS Code workflow
- **Multi-language support** (CSS, JS, HTML)
- **Beautiful, informative UI** with actionable insights
- **Performance optimized** with intelligent caching

### Impact:
- **Saves time** - No more manual feature checking
- **Increases confidence** - Clear Baseline guidance
- **Improves code quality** - Encourages modern, well-supported features
- **Educational** - Learn about new Baseline features

## 🛠️ Technical Architecture

```
src/
├── extension.ts              # Main extension entry point
├── baseline/
│   └── dataService.ts       # Web-features data integration
├── providers/
│   ├── hoverProvider.ts     # Hover tooltip functionality
│   ├── diagnostics.ts       # Visual indicators & warnings
│   └── completionProvider.ts # Smart autocomplete
└── views/
    └── sidebarProvider.ts   # Sidebar panel interface
```

## 🎥 Demo Video

*Coming soon - 3+ minute demo showcasing all features*

## 📝 License

MIT License - Open source and ready for community contributions!

## 🙏 Acknowledgments

- **Baseline Working Group** for the fantastic web-features data
- **VS Code Team** for the excellent extension API
- **Chrome DevRel** for organizing this hackathon

---

**Ready to never worry about web feature compatibility again? Install Baseline Insights and code with confidence! 🚀**
