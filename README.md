# 🎨 Yoka Canvas - Creative Designer Portfolio

<div align="center">

<img src="public\loding.gif" alt="Yoka Canvas Logo" width="200" height="200" />

**Turning your ideas into premium designs**

[![React](https://img.shields.io/badge/React-18.3.1-blue.svg)](https://reactjs.org/)
[![TypeScript](https://img.shields.io/badge/TypeScript-5.5.3-blue.svg)](https://www.typescriptlang.org/)
[![Vite](https://img.shields.io/badge/Vite-5.4.2-purple.svg)](https://vitejs.dev/)
[![Tailwind CSS](https://img.shields.io/badge/Tailwind-3.4.1-38B2AC.svg)](https://tailwindcss.com/)
[![Framer Motion](https://img.shields.io/badge/Framer%20Motion-12.15.0-black.svg)](https://www.framer.com/motion/)

[🌐 Live Demo](https://yokacanvas.com) | [📱 PWA Ready](https://yokacanvas.com) | [🎯 SEO Optimized](https://yokacanvas.com)

</div>

---

## 📋 Table of Contents

- [🎯 Project Overview](#-project-overview)
- [🚀 Features](#-features)
- [🛠️ Technology Stack](#️-technology-stack)
- [📁 Project Structure](#-project-structure)
- [⚙️ Configuration](#️-configuration)
- [🎨 Design System](#-design-system)
- [🌍 Internationalization](#-internationalization)
- [📱 Progressive Web App](#-progressive-web-app)
- [🔍 SEO & Performance](#-seo--performance)
- [🚀 Deployment](#-deployment)
- [📦 Installation & Setup](#-installation--setup)
- [🔄 Development Workflow](#-development-workflow)
- [📊 Performance Metrics](#-performance-metrics)
- [🔧 Customization](#-customization)
- [🤝 Contributing](#-contributing)
- [📄 License](#-license)

---

## 🎯 Project Overview

**Yoka Canvas** is a modern, responsive portfolio website for a creative graphic designer. Built with cutting-edge web technologies, it showcases professional design work while providing an exceptional user experience across all devices.

### 🎨 Design Philosophy

- **Minimalist & Clean**: Focus on content with elegant typography
- **Interactive Elements**: Smooth animations and micro-interactions
- **Accessibility First**: WCAG compliant with keyboard navigation
- **Performance Optimized**: Fast loading times and smooth interactions

### 🌟 Key Highlights

- **Bilingual Support**: English & Arabic with RTL layout support
- **Dark/Light Theme**: Automatic theme detection with manual toggle
- **Progressive Web App**: Installable with offline capabilities
- **SEO Optimized**: Structured data and meta tags for search engines
- **Mobile First**: Responsive design optimized for all screen sizes

---

## 🚀 Features

### 🎯 Core Features

- **Portfolio Showcase**: Interactive project gallery with filtering
- **Service Presentation**: Flip-card animations for service details
- **Contact Integration**: Direct communication channels
- **Smooth Scrolling**: Enhanced navigation experience
- **Loading Animations**: Professional splash screen and transitions

### 🌍 Internationalization

- **Dual Language Support**: English & Arabic
- **RTL Layout**: Proper right-to-left text direction
- **Cultural Adaptation**: Language-specific typography and spacing
- **Dynamic Content**: All text content translatable

### 🎨 Visual Features

- **Animated Backgrounds**: Canvas-like design elements
- **Floating Icons**: Dynamic design tool animations
- **Gradient Effects**: Custom color schemes
- **Hover Interactions**: Micro-animations throughout

### 📱 Progressive Web App

- **Installable**: Add to home screen functionality
- **Offline Ready**: Service worker implementation
- **App-like Experience**: Full-screen mode and native feel
- **Push Notifications**: Ready for future implementation

---

## 🛠️ Technology Stack

### 🎯 Frontend Framework

- **React 18.3.1**: Latest React with concurrent features
- **TypeScript 5.5.3**: Type-safe development
- **React Router DOM 7.6.3**: Client-side routing

### 🎨 Styling & Animation

- **Tailwind CSS 3.4.1**: Utility-first CSS framework
- **Framer Motion 12.15.0**: Production-ready motion library
- **Lucide React 0.344.0**: Beautiful & consistent icons
- **Custom Animations**: Tailored keyframes and transitions

### ⚡ Build Tools

- **Vite 5.4.2**: Lightning-fast build tool
- **ESLint 9.9.1**: Code quality and consistency
- **PostCSS 8.4.35**: CSS processing and optimization
- **Autoprefixer 10.4.18**: Cross-browser compatibility

### 🔧 Development Tools

- **TypeScript ESLint**: TypeScript-specific linting rules
- **React Hooks ESLint**: Hooks rules and best practices
- **React Refresh**: Hot module replacement

---

## 📁 Project Structure

```
YC port/
├── 📁 public/                    # Static assets
│   ├── 🖼️ Images (PNG files)     # Portfolio project images
│   ├── 📄 manifest.json          # PWA configuration
│   ├── 📄 robots.txt             # Search engine directives
│   └── 📄 sitemap.xml           # Site structure for SEO
├── 📁 src/
│   ├── 📁 components/
│   │   ├── 📁 layout/
│   │   │   ├── Header.tsx       # Navigation & theme controls
│   │   │   └── Footer.tsx       # Site footer
│   │   ├── 📁 sections/
│   │   │   ├── Hero.tsx         # Landing section with animations
│   │   │   ├── About.tsx        # Personal introduction
│   │   │   ├── Services.tsx     # Service offerings
│   │   │   ├── Portfolio.tsx    # Project showcase
│   │   │   └── Contact.tsx      # Contact information
│   │   └── 📁 ui/
│   │       ├── ScrollToTop.tsx  # Smooth scroll utility
│   │       ├── SplashCursor.tsx # Custom cursor effects
│   │       └── NotFound.tsx     # 404 error page
│   ├── 📁 contexts/
│   │   ├── LanguageContext.tsx  # Internationalization state
│   │   └── ThemeContext.tsx     # Dark/light theme state
│   ├── 📁 utils/
│   │   └── translations.ts      # Bilingual content management
│   ├── App.tsx                  # Main application component
│   ├── main.tsx                 # Application entry point
│   └── index.css                # Global styles
├── 📄 package.json              # Dependencies & scripts
├── 📄 tailwind.config.js       # Tailwind configuration
├── 📄 vite.config.ts           # Vite build configuration
├── 📄 vercel.json              # Deployment configuration
└── 📄 README.md                # Project documentation
```

---

## ⚙️ Configuration

### 🎨 Tailwind CSS Configuration

```javascript
// tailwind.config.js
export default {
  content: ['./index.html', './src/**/*.{js,ts,jsx,tsx}'],
  darkMode: 'class',
  theme: {
    extend: {
      colors: {
        primary: '#594998', // Main brand color
        secondary: '#FFC4A3', // Accent color
        // Additional color variations...
      },
      fontFamily: {
        giaza: ['Giaza', 'serif'],
        montserrat: ['Montserrat', 'sans-serif'],
        // Arabic font variants...
      },
      animation: {
        // Custom floating animations...
      },
    },
  },
};
```

### ⚡ Vite Configuration

```typescript
// vite.config.ts
export default defineConfig({
  base: '/',
  plugins: [react()],
  optimizeDeps: {
    exclude: ['lucide-react'],
  },
  build: {
    outDir: 'dist',
    emptyOutDir: true,
  },
});
```

### 🌐 PWA Configuration

```json
// public/manifest.json
{
  "name": "Yoka Canvas - Creative Graphic Designer",
  "short_name": "Yoka Canvas",
  "description": "Turning your ideas into premium designs",
  "start_url": "/",
  "display": "standalone",
  "background_color": "#ffffff",
  "theme_color": "#7a6ab5"
}
```

---

## 🎨 Design System

### 🎯 Color Palette

- **Primary**: `#594998` (Deep Purple)
- **Secondary**: `#FFC4A3` (Soft Coral)
- **Neutral Scale**: 50-900 gray variations
- **Dark Mode**: Inverted color scheme

### 📝 Typography

- **English**: Montserrat (Sans-serif)
- **Arabic**: Montserrat-AR (RTL optimized)
- **Display**: Giaza (Serif for headings)
- **Weights**: 300, 400, 500, 700

### 🎭 Animation System

- **Duration**: 300ms (fast), 500ms (medium), 1000ms (slow)
- **Easing**: ease-in-out for smooth transitions
- **Stagger**: 0.1s delay between elements
- **Floating**: 6-10s infinite animations

### 📱 Responsive Breakpoints

- **Mobile**: < 768px
- **Tablet**: 768px - 1024px
- **Desktop**: > 1024px
- **Large**: > 1440px

---

## 🌍 Internationalization

### 🔤 Language Support

- **English (en)**: Default language
- **Arabic (ar)**: Full RTL support
- **Dynamic Switching**: Real-time language toggle
- **Content Translation**: Complete bilingual support

### 📐 RTL Implementation

```typescript
// LanguageContext.tsx
const direction: Direction = language === 'ar' ? 'rtl' : 'ltr';

// Automatic document direction
document.documentElement.dir = direction;
document.documentElement.lang = language;
```

### 🎨 Cultural Adaptations

- **Typography**: Language-specific font families
- **Spacing**: RTL-aware margins and padding
- **Animations**: Direction-aware transitions
- **Layout**: Flexible component positioning

---

## 📱 Progressive Web App

### ✅ PWA Features

- **Installable**: Add to home screen
- **Offline Ready**: Service worker implementation
- **App-like Experience**: Full-screen mode
- **Native Feel**: Smooth transitions and gestures

### 🔧 PWA Configuration

```json
{
  "display": "standalone",
  "orientation": "portrait-primary",
  "scope": "/",
  "start_url": "/",
  "theme_color": "#7a6ab5",
  "background_color": "#ffffff"
}
```

### 📱 App Shortcuts

- **Services**: Quick access to service offerings
- **Portfolio**: Direct link to project showcase
- **Contact**: Immediate communication access

---

## 🔍 SEO & Performance

### 🎯 SEO Features

- **Meta Tags**: Comprehensive meta information
- **Structured Data**: Schema.org markup
- **Open Graph**: Social media optimization
- **Twitter Cards**: Twitter-specific meta tags
- **Sitemap**: XML sitemap for search engines
- **Robots.txt**: Search engine directives

### 📊 Performance Optimizations

- **Code Splitting**: Route-based code splitting
- **Image Optimization**: Lazy loading and compression
- **Font Loading**: Preconnect and display swap
- **Bundle Analysis**: Optimized dependency tree
- **Caching**: Strategic cache headers

### 🔍 Analytics Integration

- **Google Analytics 4**: GA4 implementation
- **Google Tag Manager**: GTM container setup
- **Event Tracking**: Custom event implementation
- **Conversion Tracking**: Goal completion monitoring

---

## 🚀 Deployment

### 🌐 Hosting Platform

- **Vercel**: Production deployment
- **Domain**: yokacanvas.com
- **SSL**: Automatic HTTPS
- **CDN**: Global content delivery

### 📦 Build Process

```bash
# Production build
npm run build

# Preview build
npm run preview

# Development server
npm run dev
```

### 🔧 Deployment Configuration

```json
// vercel.json
{
  "rewrites": [
    {
      "source": "/(.*)",
      "destination": "/index.html"
    }
  ]
}
```

---

## 📦 Installation & Setup

### 🔧 Prerequisites

- **Node.js**: 18.0.0 or higher
- **npm**: 9.0.0 or higher
- **Git**: For version control

### 🚀 Quick Start

```bash
# Clone the repository
git clone https://github.com/your-username/yoka-canvas.git

# Navigate to project directory
cd yoka-canvas

# Install dependencies
npm install

# Start development server
npm run dev

# Open in browser
open http://localhost:5173
```

### 📋 Available Scripts

```bash
npm run dev          # Start development server
npm run build        # Build for production
npm run preview      # Preview production build
npm run lint         # Run ESLint
```

### 🔧 Environment Setup

```bash
# No environment variables required
# All configuration is in config files
```

---

## 🔄 Development Workflow

### 🎯 Development Process

1. **Feature Development**: Create feature branches
2. **Code Review**: Pull request reviews
3. **Testing**: Manual and automated testing
4. **Deployment**: Automated deployment pipeline
5. **Monitoring**: Performance and error tracking

### 🛠️ Code Quality

- **ESLint**: Code style enforcement
- **TypeScript**: Type safety
- **Prettier**: Code formatting
- **Husky**: Git hooks for quality

### 📝 Commit Convention

```
feat: add new feature
fix: bug fix
docs: documentation update
style: code style changes
refactor: code refactoring
test: add tests
chore: maintenance tasks
```

---

## 📊 Performance Metrics

### ⚡ Core Web Vitals

- **LCP (Largest Contentful Paint)**: < 2.5s
- **FID (First Input Delay)**: < 100ms
- **CLS (Cumulative Layout Shift)**: < 0.1

### 📈 Performance Optimizations

- **Bundle Size**: Optimized JavaScript bundles
- **Image Optimization**: WebP format with fallbacks
- **Font Loading**: Display swap for better UX
- **Caching**: Strategic cache implementation
- **CDN**: Global content delivery network

### 🔍 Monitoring Tools

- **Google PageSpeed Insights**: Performance scoring
- **WebPageTest**: Detailed performance analysis
- **Lighthouse**: Comprehensive auditing
- **Real User Monitoring**: Actual user experience

---

## 🔧 Customization

### 🎨 Theme Customization

```typescript
// src/contexts/ThemeContext.tsx
const themes = {
  light: {
    background: '#ffffff',
    text: '#1f2937',
    primary: '#594998',
    secondary: '#FFC4A3',
  },
  dark: {
    background: '#111827',
    text: '#f9fafb',
    primary: '#7a6ab5',
    secondary: '#ffd6bd',
  },
};
```

### 🌍 Language Customization

```typescript
// src/utils/translations.ts
export const translations = {
  // Add new translation keys
  newKey: {
    en: 'English text',
    ar: 'النص العربي',
  },
};
```

### 🎭 Animation Customization

```css
/* Custom animations in tailwind.config.js */
animation: {
  'custom-float':'customFloat8sease-in-outinfinite', ;
}
,
keyframes: {
  customfloat: {
    '0%, 100%': {
      transform: 'translate(0, 0)';
    }
    ,
    '50%': {
      transform: 'translate(10px, -10px)';
    }
  }
}
```

---

## 🤝 Contributing

### 📋 Contribution Guidelines

1. **Fork the repository**
2. **Create a feature branch**: `git checkout -b feature/amazing-feature`
3. **Commit your changes**: `git commit -m 'feat: add amazing feature'`
4. **Push to the branch**: `git push origin feature/amazing-feature`
5. **Open a Pull Request**

### 🛠️ Development Setup

```bash
# Install dependencies
npm install

# Start development server
npm run dev

# Run linting
npm run lint

# Build for production
npm run build
```

### 📝 Code Standards

- **TypeScript**: Strict type checking
- **ESLint**: Code quality rules
- **Prettier**: Code formatting
- **Conventional Commits**: Commit message format

---

## 📄 License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.

---

## 🙏 Acknowledgments

- **React Team**: For the amazing framework
- **Vite Team**: For the lightning-fast build tool
- **Tailwind CSS**: For the utility-first CSS framework
- **Framer Motion**: For the smooth animations
- **Lucide**: For the beautiful icons

---

<div align="center">

[🌐 Website](https://yokacanvas.com) | [📧 Contact](mailto:contact@yokacanvas.com) | [💼 Portfolio](https://behance.net/yokacanvas)

</div>

---

<div align="center">
  <p>Made with 🤍 by  <strong>  BnRamadan</strong> </p>
</div>
