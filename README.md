# BlendCSS 🎨

> A modern, hybrid CSS framework that seamlessly blends classless semantic HTML styling with powerful utility classes and customizable components.

[![Version](https://img.shields.io/badge/version-1.0.0--dev-orange.svg)](https://github.com/openabir/blend-css)
[![License](https://img.shields.io/badge/license-MIT-green.svg)](https://opensource.org/licenses/MIT)
[![CSS](https://img.shields.io/badge/CSS-3-blue.svg)](https://www.w3.org/Style/CSS/)
[![SCSS](https://img.shields.io/badge/SCSS-Sass-pink.svg)](https://sass-lang.com/)
[![Development](https://img.shields.io/badge/status-in%20development-yellow.svg)](https://github.com/openabir/blend-css)

## ⚠️ Development Status

BlendCSS is currently under active development by a solo developer. The framework is not yet ready for production use. I'm working hard to deliver a comprehensive solution that combines the best of classless, utility-first, and component-based CSS approaches.

## ✨ What Makes BlendCSS Different?

BlendCSS is a **hybrid approach** that combines the best of multiple CSS methodologies:

- 🎯 **Classless** - Beautiful styling with zero classes required
- ⚡ **Utilities** - Atomic classes for rapid development
- 🧩 **Components** - Pre-built patterns for complex UI elements
- 🌙 **Dark Mode** - Built-in light/dark theme support
- 📱 **Responsive** - Mobile-first design principles
- 🎨 **Customizable** - CSS custom properties for easy theming
- 🔧 **Modern** - Built with latest CSS features and best practices

## 🏗️ Architecture

BlendCSS follows a **layered architecture** that allows you to use as much or as little as you need:

```
┌─ 1. Base Layer ─────────────────┐
│  • Complete CSS Reset           │
│  • CSS Custom Properties        │
│  • Typography Foundation        │
└─────────────────────────────────┘
┌─ 2. Classless Layer ────────────┐
│  • Semantic HTML Styling        │
│  • Zero-class layouts           │
│  • Beautiful defaults           │
└─────────────────────────────────┘
┌─ 3. Utilities Layer ────────────┐
│  • Spacing (margin, padding)    │
│  • Flexbox & Grid               │
│  • Colors & Typography          │
└─────────────────────────────────┘
┌─ 4. Components Layer ───────────┐
│  • Buttons & Forms              │
│  • Cards & Modals               │
│  • Navigation & Layout          │
└─────────────────────────────────┘
┌─ 5. Themes Layer ───────────────┐
│  • Light & Dark Modes           │
│  • Custom Color Schemes         │
│  • Brand Customization          │
└─────────────────────────────────┘
```

## 📁 Project Structure

```
BlendCSS/
├── scss/
│   ├── main.scss                 # Main entry point
│   ├── base/
│   │   ├── _reset.scss           # Complete CSS reset
│   │   ├── _variables.scss       # CSS custom properties
│   │   └── _typography.scss      # Typography foundation
│   ├── classless/
│   │   ├── _elements.scss        # Semantic HTML styling
│   │   └── _layout.scss          # Layout defaults
│   ├── utilities/
│   │   ├── _spacing.scss         # Margin/padding utilities
│   │   ├── _flex.scss            # Flexbox utilities
│   │   ├── _grid.scss            # Grid utilities
│   │   ├── _colors.scss          # Color utilities
│   │   └── _typography.scss      # Typography utilities
│   ├── components/
│   │   ├── _buttons.scss         # Button components
│   │   ├── _cards.scss           # Card components
│   │   ├── _forms.scss           # Form components
│   │   ├── _modals.scss          # Modal components
│   │   └── _navbar.scss          # Navigation components
│   └── themes/
│       ├── _light.scss           # Light theme
│       └── _dark.scss            # Dark theme
├── css/
│   └── blend.css                 # Compiled CSS
├── examples/
│   ├── classless.html            # Classless examples
│   ├── utilities.html            # Utility examples
│   └── hybrid.html               # Combined approach
└── docs/                         # Documentation
```

## 🎨 Design System

### Core Features

**Color System**

- Comprehensive color palettes with 50-950 scales
- Semantic colors for success, warning, error, and info states
- Automatic dark mode support
- CSS custom properties for easy customization

**Typography**

- Modern font stacks with system font fallbacks
- Responsive typography scale
- Perfect line heights and spacing
- Support for display and body text

**Spacing System**

- Based on 4px grid system
- Consistent spacing scale from 0 to 96 units
- Calculated using CSS custom properties

**Layout System**

- Container sizes for different breakpoints
- Z-index scale for layering components
- Responsive breakpoint values

## 🌙 Dark Mode

BlendCSS includes built-in dark mode support with both automatic system preference detection and manual toggle options.

## 📱 Responsive Design

Mobile-first approach with comprehensive breakpoint system:

- `xs`: 320px
- `sm`: 480px
- `md`: 768px
- `lg`: 1024px
- `xl`: 1280px
- `2xl`: 1536px

## 🧪 Browser Support

BlendCSS targets all modern browsers:

- ✅ Chrome 88+
- ✅ Firefox 85+
- ✅ Safari 14+
- ✅ Edge 88+

Features include progressive enhancement with graceful degradation for older browsers.

## 🛠️ Development Setup

```bash
# Clone the repository
git clone https://github.com/openabir/blend-css.git
cd blend-css

# Install dependencies
npm install

# Start development
npm run dev

# Build for production
npm run build

# Watch for changes
npm run watch
```

## 🤝 Contributing

I welcome contributions from developers of all skill levels! While BlendCSS is a solo project, I believe in the power of community collaboration and would love your help making it better.

### Ways to Help

- 🐛 **Report Bugs** - Help me identify and fix issues
- 💡 **Suggest Features** - Share ideas for new functionality
- 📝 **Improve Documentation** - Help make the docs clearer
- 🔧 **Submit Code** - Fix bugs or implement new features
- 🎨 **Design Input** - Contribute to UI/UX decisions
- 🧪 **Testing** - Help test across different browsers and devices
- 📢 **Spread the Word** - Share the project with others

### Getting Started

1. **Fork the repository** on GitHub
2. **Clone your fork** locally
3. **Create a feature branch** from `main`
4. **Make your changes** following the guidelines below
5. **Test your changes** thoroughly
6. **Submit a pull request** with a clear description

### Development Guidelines

Since I'm working solo, maintaining consistency is crucial:

- Follow existing code style and conventions
- Write clear, descriptive commit messages
- Comment complex logic and design decisions
- Keep lines under 100 characters when possible
- Use meaningful variable and mixin names
- Test responsive behavior on different screen sizes

### Code Style

- Use 2 spaces for indentation
- Follow BEM naming convention for CSS classes
- Use semantic HTML5 elements
- Prioritize accessibility
- Write mobile-first responsive CSS

### Pull Request Process

1. Ensure your code follows the style guidelines
2. Update documentation if needed
3. Test across multiple browsers
4. Provide clear description of changes
5. Be patient - as a solo developer, review may take time

### Reporting Issues

When reporting bugs, please include:

- Browser version and operating system
- Steps to reproduce the issue
- Expected vs actual behavior
- Screenshots if applicable
- Minimal code example demonstrating the issue

### Feature Requests

I love hearing new ideas! When suggesting features:

- Explain the use case and problem it solves
- Provide examples of how it would be used
- Consider how it fits with the existing architecture
- Check if similar functionality already exists

## 👤 About the Developer

**[openabir](https://github.com/openabir)** - Creator & Solo Developer

I'm passionate about creating tools that make web development more enjoyable and efficient. BlendCSS is my attempt to solve the common dilemma of choosing between different CSS approaches by combining the best of all worlds.

### Why I Built BlendCSS

As a developer, I've always been torn between the simplicity of classless CSS frameworks and the flexibility of utility-first approaches. I wanted something that could:

- Work beautifully out of the box without any classes
- Provide utility classes when I need precise control
- Include pre-built components for common patterns
- Support modern features like dark mode
- Be easily customizable for different projects

BlendCSS is my solution to this challenge.

### Connect With Me

- 🐙 GitHub: [@openabir](https://github.com/openabir)
- 💬 Discussions: [Project Discussions](https://github.com/openabir/blend-css/discussions)
- 🐛 Issues: [Report Issues](https://github.com/openabir/blend-css/issues)

## 📊 Project Status

### Current Progress

- ✅ **Foundation Layer** - CSS Reset & Variables (Complete)
- 🚧 **Base Layer** - Typography & Core Styles (In Progress)
- ⏳ **Classless Layer** - Semantic HTML Styling (Planned)
- ⏳ **Utilities Layer** - Atomic Classes (Planned)
- ⏳ **Components Layer** - UI Components (Planned)
- ⏳ **Themes Layer** - Light/Dark Modes (Planned)

### Development Roadmap

**Phase 1: Foundation** (Current)

- Complete CSS reset system
- Establish design tokens and variables
- Set up build process and tooling

**Phase 2: Core Styling**

- Implement classless semantic HTML styling
- Create comprehensive utility class system
- Establish responsive grid system

**Phase 3: Components**

- Build essential UI components
- Create interactive elements
- Implement advanced layout patterns

**Phase 4: Theming**

- Complete dark mode implementation
- Create theme customization system
- Build color scheme variants

**Phase 5: Polish & Release**

- Performance optimization
- Bundle size reduction
- Browser compatibility testing
- Documentation and examples

### Timeline

This is a passion project developed in my spare time. While I don't have strict deadlines, I'm committed to steady progress and regular updates.

## 📄 License

MIT License - see the [LICENSE](LICENSE) file for details.

This means you're free to use, modify, and distribute BlendCSS in your projects, both personal and commercial.

## 🙏 Acknowledgments

- Inspired by [Tailwind CSS](https://tailwindcss.com/) utility-first approach
- Influenced by [Pico CSS](https://picocss.com/) classless philosophy
- Built with [Sass](https://sass-lang.com/) preprocessing
- Reset based on modern CSS reset practices

## 🔗 Links

- 📖 [Documentation](https://blendcss.dev) (Coming Soon)
- 🎮 [Playground](https://codepen.io/collection/blendcss) (Coming Soon)
- 💬 [Discussions](https://github.com/openabir/blend-css/discussions)
- 🐛 [Issues](https://github.com/openabir/blend-css/issues)

---

<div align="center">
    <p>Made with ❤️ by <a href="https://github.com/openabir">openabir</a></p>
    <p>
        <a href="https://github.com/openabir/blend-css/stargazers">⭐ Star us on GitHub</a> •
        <a href="https://github.com/openabir/blend-css/fork">🍴 Fork the project</a> •
        <a href="https://github.com/openabir/blend-css/discussions">💬 Join the discussion</a>
    </p>
</div>
