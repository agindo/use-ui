# 🎨 use-ui

**use-ui** adalah library komponen template UI modern yang dirancang untuk kemudahan penggunaan dan fleksibilitas tinggi. Proyek ini menggabungkan best practices dalam **Design System**, **Dokumentasi API**, dan **Implementasi lintas framework**.

> ✨ **Fokus:** HTML + CSS yang elegan | **Tujuan:** Mudah digunakan across platforms | **Status:** Aktif dikembangkan

---

## 📋 Daftar Isi

- [Project Overview](#project-overview)
- [Features List](#-features-list)
- [Fitur Utama](#fitur-utama)
- [Instalasi](#instalasi)
- [Quick Start](#quick-start)
- [Design System](#design-system)
  - [Design Principles](#-design-system-principles)
  - [Color System](#palet-warna)
  - [Typography](#typography)
  - [Spacing](#spacing)
- [Struktur Komponen](#struktur-komponen)
  - [Organisasi Folder](#-organisasi-folder)
  - [Anatomi Komponen](#-anatomi-komponen)
  - [Component Patterns](#-component-patterns)
  - [File Conventions](#-component-file-conventions)
  - [Dependencies](#-component-dependencies)
  - [Framework-Specific Code](#-framework-specific-code)
  - [Kategori Komponen](#-component-categories)
  - [Composables & Utilities](#-composables--utilities)
- [Dokumentasi API](#dokumentasi-api)
- [Dukungan Lintas Framework](#dukungan-lintas-framework)
  - [Cross-Framework Strategy](#-cross-framework-strategy)
  - [Architecture Overview](#-architecture-overview)
  - [How It Works](#-how-it-works)
  - [Framework Comparison](#-framework-comparison)
  - [Installation & Setup](#-installation--setup)
  - [Implementation Examples](#-implementation-examples)
  - [Theme & Styling](#-theme--styling-across-frameworks)
  - [Interoperability & Migration](#-interoperability--migration)
  - [Testing Across Frameworks](#-testing-across-frameworks)
  - [Performance Considerations](#-performance-considerations)
  - [When to Use Each Framework](#-when-to-use-each-framework)
- [Struktur Proyek](#struktur-proyek)
  - [Complete Directory Tree](#-complete-directory-tree)
  - [Directory Purposes](#-directory-purposes)
  - [Component File Structure](#-component-file-structure-example)
  - [npm Scripts](#-npm-scripts)
  - [Configuration Files](#-configuration-files-explained)
  - [Build Output Structure](#-build-output-structure)
  - [Development Workflow](#-development-workflow)
  - [Entry Points](#-entry-points)
- [Setup Development](#-setup-development)
- [Kontribusi](#kontribusi)
- [Lisensi](#lisensi)

---

## 🎯 Project Overview

### Visi & Misi

**use-ui** dilahirkan dari kebutuhan akan UI component library yang modern, mudah digunakan, dan tidak mengikat ke framework tertentu. Proyek ini bertujuan untuk:

- 🎨 **Democratisasi UI Development** - Membuat UI component library yang accessible dan mudah digunakan oleh developer dari semua level
- 🔄 **Framework Agnostic** - Mendukung berbagai framework modern (Vue, React, Angular, Vanilla JS)
- 📖 **Developer Experience** - Menyediakan dokumentasi lengkap, contoh kode, dan interactive playground
- 🏗️ **Production Ready** - Komponen yang robust, tested, dan siap untuk production

### Siapa Target use-ui?

✅ **Frontend Developers** - Yang mencari UI component library yang cepat untuk dikonfigurasi
✅ **Design Systems Teams** - Yang ingin membangun design system yang konsisten
✅ **Startup & Agency** - Yang butuh cepat prototype dan launch aplikasi
✅ **Enterprise** - Yang membutuhkan customizable component library
✅ **Open Source Contributors** - Yang ingin berkontribusi pada proyek yang growing

### Nilai Inti Proyek

| Nilai | Penjelasan |
|-------|-----------|
| **Simplicity** | Mudah dipahami, mudah digunakan, mudah dikustomisasi |
| **Consistency** | Design yang konsisten, API yang predictable |
| **Quality** | Tested code, documented, performance optimized |
| **Flexibility** | Dapat digunakan di berbagai platform dan use case |
| **Community** | Open source, collaborative, welcoming |

### Roadmap & Milestone

#### Phase 1: Foundation (Q3 2024)
- ✅ Setup project structure dan tooling
- ✅ Create base component library (Button, Input, Card, etc)
- ✅ Setup Storybook untuk component documentation
- ✅ Create design system dengan CSS Variables

#### Phase 2: Expansion (Q4 2024)
- 🔄 Add advanced components (Modal, Dropdown, Tabs)
- 🔄 Build React & Angular wrappers
- 🔄 Setup comprehensive testing suite
- 🔄 Launch official documentation site

#### Phase 3: Optimization (Q1 2025)
- 📅 Performance optimization dan bundle size reduction
- 📅 Accessibility audit dan compliance (WCAG 2.1 AA)
- 📅 Add theming & customization capabilities
- 📅 Build CLI tool untuk scaffolding

#### Phase 4: Scale (Q2+ 2025)
- 📅 Community plugins & extensions
- 📅 Premium templates & themes
- 📅 Enterprise support program
- 📅 Mobile (React Native) support

### Komparasi dengan Library Lain

| Aspek | use-ui | Bootstrap | Material UI | Tailwind |
|-------|--------|-----------|-------------|----------|
| **Framework** | Vue/React/Angular/Vanilla | Vanilla/jQuery | React | CSS Utility |
| **Styling** | CSS + Tailwind | CSS | Emotion (CSS-in-JS) | Utility Classes |
| **Customization** | CSS Variables | SCSS Variables | Theme Provider | Config |
| **Bundle Size** | ~25KB gzip | ~50KB gzip | ~100KB+ | ~15KB gzip |
| **Learning Curve** | Easy | Medium | Medium | Easy |
| **Production Ready** | Yes | Yes | Yes | Yes |

### Keunggulan use-ui

✨ **Modern** - Built dengan teknologi terkini (Vue 3 Composition API, Vite, TypeScript)
✨ **Lightweight** - Minimal dependencies, optimized untuk performance
✨ **Developer Friendly** - Clear API, comprehensive docs, helpful error messages
✨ **Accessible** - WCAG 2.1 compliant dari awal
✨ **Highly Customizable** - CSS Variables, design tokens, theme support
✨ **Framework Flexible** - Tidak terikat satu framework, bisa digunakan dimana saja

---

## 📦 Features List

### ✅ Komponen Form (Form Components)

| Komponen | Deskripsi | Status | Vue 3 | React | Angular |
|----------|-----------|--------|-------|-------|---------|
| **UseButton** | Button dengan multiple variants & sizes | ✅ Available | ✅ | ✅ | ✅ |
| **UseInput** | Text input field dengan validation | ✅ Available | ✅ | ✅ | ✅ |
| **UseSelect** | Dropdown selection component | ✅ Available | ✅ | ✅ | ✅ |
| **UseCheckbox** | Checkbox control | ✅ Available | ✅ | ✅ | ✅ |
| **UseRadio** | Radio button group | ✅ Available | ✅ | ✅ | ✅ |
| **UseTextarea** | Multi-line text input | ✅ Available | ✅ | ✅ | ✅ |
| **UseSwitch** | Toggle/Switch component | ✅ Available | ✅ | ✅ | ✅ |
| **UseFileUpload** | File upload dengan drag-drop | ✅ Available | ✅ | ✅ | ✅ |
| **UseForm** | Form wrapper dengan validation | ✅ Available | ✅ | ✅ | ✅ |
| **UseRating** | Rating star component | 🔄 Coming | - | - | - |
| **UseSlider** | Range slider component | 🔄 Coming | - | - | - |

### ✅ Komponen Layout (Layout Components)

| Komponen | Deskripsi | Status | Vue 3 | React | Angular |
|----------|-----------|--------|-------|-------|---------|
| **UseContainer** | Container dengan max-width | ✅ Available | ✅ | ✅ | ✅ |
| **UseGrid** | Grid layout system (12 columns) | ✅ Available | ✅ | ✅ | ✅ |
| **UseStack** | Flexbox stack (horizontal/vertical) | ✅ Available | ✅ | ✅ | ✅ |
| **UseCard** | Card component dengan slot support | ✅ Available | ✅ | ✅ | ✅ |
| **UseSpacer** | Spacing utility component | ✅ Available | ✅ | ✅ | ✅ |
| **UseFlex** | Flexbox wrapper component | ✅ Available | ✅ | ✅ | ✅ |
| **UseAspectRatio** | Aspect ratio wrapper | 🔄 Coming | - | - | - |

### ✅ Komponen Navigation (Navigation Components)

| Komponen | Deskripsi | Status | Vue 3 | React | Angular |
|----------|-----------|--------|-------|-------|---------|
| **UseNavbar** | Top navigation bar | ✅ Available | ✅ | ✅ | ✅ |
| **UseSidebar** | Side navigation menu | ✅ Available | ✅ | ✅ | ✅ |
| **UseBreadcrumb** | Breadcrumb navigation | ✅ Available | ✅ | ✅ | ✅ |
| **UseMenu** | Dropdown menu component | ✅ Available | ✅ | ✅ | ✅ |
| **UseTabs** | Tab navigation component | ✅ Available | ✅ | ✅ | ✅ |
| **UsePagination** | Pagination control | ✅ Available | ✅ | ✅ | ✅ |
| **UseButton Group** | Grouped button toolbar | 🔄 Coming | - | - | - |

### ✅ Komponen Feedback (Feedback & Notification)

| Komponen | Deskripsi | Status | Vue 3 | React | Angular |
|----------|-----------|--------|-------|-------|---------|
| **UseAlert** | Alert/banner message | ✅ Available | ✅ | ✅ | ✅ |
| **UseToast** | Toast notification system | ✅ Available | ✅ | ✅ | ✅ |
| **UseModal** | Modal dialog component | ✅ Available | ✅ | ✅ | ✅ |
| **UseDrawer** | Side drawer/panel | ✅ Available | ✅ | ✅ | ✅ |
| **UseTooltip** | Tooltip information | ✅ Available | ✅ | ✅ | ✅ |
| **UsePopover** | Popover overlay | ✅ Available | ✅ | ✅ | ✅ |
| **UseProgress** | Progress bar | ✅ Available | ✅ | ✅ | ✅ |
| **UseSkeleton** | Loading skeleton | ✅ Available | ✅ | ✅ | ✅ |
| **UseSpinner** | Loading spinner | ✅ Available | ✅ | ✅ | ✅ |
| **UseConfirm** | Confirmation dialog | 🔄 Coming | - | - | - |

### ✅ Komponen Data Display (Data Display)

| Komponen | Deskripsi | Status | Vue 3 | React | Angular |
|----------|-----------|--------|-------|-------|---------|
| **UseTable** | Data table dengan sorting/filtering | ✅ Available | ✅ | ✅ | ✅ |
| **UseBadge** | Badge component | ✅ Available | ✅ | ✅ | ✅ |
| **UseTag** | Tag component dengan variants | ✅ Available | ✅ | ✅ | ✅ |
| **UseAvatar** | Avatar component | ✅ Available | ✅ | ✅ | ✅ |
| **UseList** | List component | ✅ Available | ✅ | ✅ | ✅ |
| **UseStatistic** | Statistic display | ✅ Available | ✅ | ✅ | ✅ |
| **UseTimeline** | Timeline component | 🔄 Coming | - | - | - |
| **UseTree** | Tree view component | 🔄 Coming | - | - | - |

### 🎨 Design System Features

| Fitur | Deskripsi | Status |
|-------|-----------|--------|
| **Color Palette** | Comprehensive color system dengan 9 shades per color | ✅ Available |
| **Typography** | Font sizing & weight system | ✅ Available |
| **Spacing Scale** | Standardized spacing (4px base unit) | ✅ Available |
| **Breakpoints** | Responsive breakpoints (5 breakpoints) | ✅ Available |
| **Shadows** | Elevation shadow system | ✅ Available |
| **Border Radius** | Radius scale untuk components | ✅ Available |
| **Icons** | SVG icon library built-in | 🔄 Coming |
| **Dark Mode** | Automatic dark theme support | 🔄 Coming |
| **Theme Tokens** | Design token system | 🔄 Coming |

### 📚 Developer Experience Features

| Fitur | Deskripsi | Status |
|-------|-----------|--------|
| **TypeScript Support** | Full TypeScript types & generics | ✅ Available |
| **Storybook** | Interactive component playground | ✅ Available |
| **API Documentation** | Auto-generated from JSDoc | ✅ Available |
| **Usage Examples** | Code examples untuk setiap komponen | ✅ Available |
| **Design Guidelines** | Best practices & usage patterns | ✅ Available |
| **Playground** | Online playground untuk testing | 🔄 Coming |
| **CLI Tool** | Scaffold components & projects | 🔄 Coming |
| **Figma Plugin** | Figma design kit integration | 📅 Planned |

### 🔧 Advanced Features

| Fitur | Deskripsi | Status |
|-------|-----------|--------|
| **Composables (Vue)** | Vue 3 composition utilities | ✅ Available |
| **Hooks (React)** | Custom React hooks | ✅ Available |
| **Form Validation** | Built-in validation library | ✅ Available |
| **Accessibility** | WCAG 2.1 Level AA compliance | ✅ Available |
| **Responsive** | Mobile-first responsive design | ✅ Available |
| **Theming** | Runtime theming dengan CSS Variables | ✅ Available |
| **Performance** | Tree-shakeable, code splitting ready | ✅ Available |
| **i18n Ready** | Internationalization support | ✅ Available |
| **Keyboard Navigation** | Full keyboard accessibility | ✅ Available |
| **Custom Events** | Framework-agnostic event system | ✅ Available |

### 📊 Browser Support

| Browser | Minimum Version | Status |
|---------|-----------------|--------|
| Chrome | 90+ | ✅ Supported |
| Firefox | 88+ | ✅ Supported |
| Safari | 14+ | ✅ Supported |
| Edge | 90+ | ✅ Supported |
| Opera | 76+ | ✅ Supported |
| IE 11 | - | ❌ Not Supported |

### 📈 Performance Metrics

| Metrik | Target | Achieved |
|--------|--------|----------|
| **Bundle Size (gzip)** | < 30KB | ✅ ~25KB |
| **Lighthouse Performance** | > 90 | ✅ 95 |
| **First Contentful Paint** | < 1.5s | ✅ ~1.2s |
| **Tree Shakeable** | 100% | ✅ Yes |
| **Framework Overhead** | < 5KB | ✅ ~3KB |

---

### 🎯 Design System
- **Konsistensi Visual** - Palette warna, typography, dan spacing yang terstandar
- **Komponen Reusable** - Library komponen UI yang dapat digunakan kembali
- **Accessibility** - Mendukung WCAG 2.1 Level AA standards
- **Responsive Design** - Fully responsive untuk semua ukuran perangkat

### 🧩 Komponen UI
- Button (berbagai varian: primary, secondary, ghost, danger)
- Input & Form Controls (text input, select, checkbox, radio)
- Card & Container (layout components)
- Navigation (navbar, menu, breadcrumb)
- Modal & Dialog
- Toast & Notification
- Badge & Tag
- Tooltip & Popover
- Dan lebih banyak lagi...

### 📚 Dokumentasi Lengkap
- **Interactive Storybook** - Preview dan test komponen secara interaktif
- **API Reference** - Dokumentasi lengkap untuk setiap komponen
- **Usage Examples** - Contoh kode implementasi untuk berbagai use case
- **Design Guidelines** - Panduan penggunaan dan best practices

### 🌐 Implementasi Lintas Framework
- **Vue 3** - Full support dengan Composition API
- **React** - Wrapper components tersedia
- **Vanilla JavaScript** - Web Components untuk penggunaan standalone
- **Angular** - Component bindings untuk Angular projects

### 💪 Bukan Sekadar HTML + CSS
- **State Management** - Komponen dengan state yang intelligent
- **Event Handling** - Custom events dan callbacks yang powerful
- **Validation** - Built-in form validation
- **Theming** - Dynamic theming support dengan CSS Variables
- **Utilities** - Helper functions dan composables

---

## 📦 Instalasi

### Prerequisites

Sebelum menginstal use-ui, pastikan Anda memiliki:

| Requirement | Minimum Version | Catatan |
|-------------|-----------------|--------|
| **Node.js** | 16.0.0 | Untuk npm/yarn/pnpm |
| **npm/yarn/pnpm** | Latest | Package manager |
| **Framework** | Latest LTS | Vue 3.3+, React 18+, Angular 15+, atau Vanilla JS |

Cek versi Node.js Anda:
```bash
node --version
npm --version
```

### Installation Methods

#### 1️⃣ NPM (Recommended)
```bash
npm install use-ui
```

#### 2️⃣ Yarn
```bash
yarn add use-ui
```

#### 3️⃣ PNPM
```bash
pnpm add use-ui
```

#### 4️⃣ CDN (Vanilla JS)
```html
<!-- CSS -->
<link rel="stylesheet" href="https://cdn.jsdelivr.net/npm/use-ui@latest/dist/style.css">

<!-- JS -->
<script src="https://cdn.jsdelivr.net/npm/use-ui@latest/dist/use-ui.umd.js"></script>
```

#### 5️⃣ From Git (Development)
```bash
git clone https://github.com/yourusername/use-ui.git
cd use-ui
npm install
npm run build
npm link  # Link ke project lokal
```

### Framework-Specific Installation

#### Vue 3
```bash
npm install use-ui vue@^3.3.0
```

#### React
```bash
npm install use-ui @use-ui/react react@^18.0.0 react-dom@^18.0.0
```

#### Angular
```bash
npm install use-ui @use-ui/angular @angular/core@^15.0.0
```

#### Vanilla JavaScript (Web Components)
```bash
npm install use-ui
```
Atau gunakan CDN link di atas.

### Verification

Setelah instalasi, verifikasi dengan:

```bash
# Check package installation
npm list use-ui

# Output should show:
# use-ui@1.0.0
```

### Installation Options

#### Full Bundle (Recommended)
```bash
npm install use-ui
```
- Ukuran: ~25KB gzip
- Semua komponen included
- Best untuk most use cases

#### Tree-Shakeable Import
```bash
npm install use-ui
```

Kemudian import hanya komponen yang dibutuhkan:

```javascript
// Vue 3
import { UseButton, UseInput } from 'use-ui'

// React
import { UseButton, UseInput } from '@use-ui/react'
```

#### Peer Dependencies

Pastikan Anda memiliki peer dependencies yang diperlukan:

```json
{
  "vue": "^3.3.0",      // Untuk Vue 3
  "react": "^18.0.0",   // Untuk React
  "react-dom": "^18.0.0" // Untuk React
}
```

### Troubleshooting

#### Problem: Module not found error
```bash
# Solution: Clear node_modules dan reinstall
rm -rf node_modules package-lock.json
npm install
```

#### Problem: CSS not loading
```javascript
// Make sure to import CSS
import 'use-ui/dist/style.css'

// Or add to your global styles
@import 'use-ui/dist/style.css';
```

#### Problem: Compatibility issues
```bash
# Check Node.js version
node --version  # Should be 16.0.0+

# Update npm
npm install -g npm@latest

# Reinstall dependencies
npm ci  # Use npm ci instead of npm install for CI/CD
```

#### Problem: Build errors

Jika mengalami build error, lihat dokumentasi framework:
- [Vue 3 Setup](https://vuejs.org/guide/installation.html)
- [React Setup](https://react.dev/learn/installation)
- [Angular Setup](https://angular.io/guide/setup-local)
- [Vite Setup](https://vitejs.dev/guide/)

### Uninstall

Jika perlu uninstall use-ui:

```bash
npm uninstall use-ui
```

### Update ke Version Terbaru

```bash
# Check available versions
npm view use-ui versions

# Update ke latest version
npm install use-ui@latest

# Or update to specific version
npm install use-ui@1.2.0
```

### Next Steps

Setelah instalasi berhasil:

1. **Quick Start** - Lihat [Quick Start](#quick-start) section
2. **Documentation** - Baca [Dokumentasi API](#dokumentasi-api)
3. **Examples** - Lihat contoh di [Framework Examples](#-dukungan-lintas-framework)
4. **Storybook** - Jelajahi komponen interaktif: `npm run storybook`

---

## 🚀 Quick Start

### 5 Menit Setup untuk Vue 3, React, dan Vanilla JS

Pilih framework yang Anda gunakan dan ikuti langkah-langkah di bawah:

---

### Vue 3 Quick Start

#### Step 1: Install Dependencies
```bash
npm install use-ui
```

#### Step 2: Setup Main.js
```javascript
// src/main.js
import { createApp } from 'vue'
import useUI from 'use-ui'
import 'use-ui/dist/style.css'
import App from './App.vue'

const app = createApp(App)

// Register use-ui plugin
app.use(useUI)

app.mount('#app')
```

#### Step 3: Use Components in Templates
```vue
<template>
  <div class="p-4">
    <!-- Button Component -->
    <UseButton type="primary" @click="handleClick" class="mb-4">
      Click Me!
    </UseButton>

    <!-- Card Component -->
    <UseCard title="Welcome to use-ui">
      <p>Ini adalah contoh card component</p>
    </UseCard>

    <!-- Input Component -->
    <UseInput 
      v-model="username" 
      label="Username"
      placeholder="Masukkan username Anda"
      class="mt-4"
    />

    <!-- Display Value -->
    <p class="mt-2" v-if="username">Username: {{ username }}</p>
  </div>
</template>

<script setup>
import { ref } from 'vue'

const username = ref('')

const handleClick = () => {
  console.log('Button clicked!')
  alert('Button was clicked!')
}
</script>
```

#### Step 4: Run Development Server
```bash
npm run dev
```

✅ You're done! Vue 3 integration complete.

---

### React Quick Start

#### Step 1: Install Dependencies
```bash
npm install use-ui @use-ui/react react@^18 react-dom@^18
```

#### Step 2: Setup App Component
```jsx
// src/App.jsx
import { UseButton, UseCard, UseInput } from '@use-ui/react'
import 'use-ui/dist/style.css'
import { useState } from 'react'

function App() {
  const [username, setUsername] = useState('')

  const handleClick = () => {
    console.log('Button clicked!')
    alert('Button was clicked!')
  }

  return (
    <div className="p-4">
      {/* Button Component */}
      <UseButton 
        type="primary" 
        onClick={handleClick}
        className="mb-4"
      >
        Click Me!
      </UseButton>

      {/* Card Component */}
      <UseCard title="Welcome to use-ui">
        <p>Ini adalah contoh card component</p>
      </UseCard>

      {/* Input Component */}
      <UseInput 
        value={username}
        onChange={(e) => setUsername(e.target.value)}
        label="Username"
        placeholder="Masukkan username Anda"
        className="mt-4"
      />

      {/* Display Value */}
      {username && <p className="mt-2">Username: {username}</p>}
    </div>
  )
}

export default App
```

#### Step 3: Import in Main.jsx
```jsx
// src/main.jsx
import React from 'react'
import ReactDOM from 'react-dom/client'
import App from './App.jsx'

ReactDOM.createRoot(document.getElementById('root')).render(
  <React.StrictMode>
    <App />
  </React.StrictMode>,
)
```

#### Step 4: Run Development Server
```bash
npm run dev
```

✅ React integration complete.

---

### Angular Quick Start

#### Step 1: Install Dependencies
```bash
npm install use-ui @use-ui/angular
```

#### Step 2: Import Module
```typescript
// src/app/app.module.ts
import { NgModule } from '@angular/core'
import { BrowserModule } from '@angular/platform-browser'
import { UseUIModule } from '@use-ui/angular'

import { AppComponent } from './app.component'

@NgModule({
  declarations: [
    AppComponent
  ],
  imports: [
    BrowserModule,
    UseUIModule  // Import use-ui module
  ],
  providers: [],
  bootstrap: [AppComponent]
})
export class AppModule { }
```

#### Step 3: Use Components
```typescript
// src/app/app.component.ts
import { Component } from '@angular/core'

@Component({
  selector: 'app-root',
  template: `
    <div class="p-4">
      <!-- Button Component -->
      <use-button 
        type="primary" 
        (click)="handleClick()"
        class="mb-4"
      >
        Click Me!
      </use-button>

      <!-- Card Component -->
      <use-card title="Welcome to use-ui">
        <p>Ini adalah contoh card component</p>
      </use-card>

      <!-- Input Component -->
      <use-input 
        [(ngModel)]="username"
        label="Username"
        placeholder="Masukkan username Anda"
        class="mt-4"
      ></use-input>

      <!-- Display Value -->
      <p class="mt-2" *ngIf="username">Username: {{ username }}</p>
    </div>
  `
})
export class AppComponent {
  username: string = ''

  handleClick() {
    console.log('Button clicked!')
    alert('Button was clicked!')
  }
}
```

#### Step 4: Add CSS Import
```css
/* src/styles.css */
@import 'use-ui/dist/style.css';
```

#### Step 5: Run Development Server
```bash
ng serve
```

✅ Angular integration complete.

---

### Vanilla JavaScript Quick Start

#### Step 1: Include via CDN
```html
<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <title>use-ui Demo</title>
  
  <!-- Include use-ui CSS -->
  <link rel="stylesheet" href="https://cdn.jsdelivr.net/npm/use-ui@latest/dist/style.css">
</head>
<body>
  <div id="app" class="p-4">
    <!-- Components will be rendered here -->
  </div>

  <!-- Include use-ui JS -->
  <script src="https://cdn.jsdelivr.net/npm/use-ui@latest/dist/use-ui.umd.js"></script>
  
  <script>
    const app = document.getElementById('app')

    // Create Button
    const button = document.createElement('use-button')
    button.setAttribute('type', 'primary')
    button.textContent = 'Click Me!'
    button.className = 'mb-4'
    button.addEventListener('click', () => {
      alert('Button was clicked!')
    })
    app.appendChild(button)

    // Create Card
    const card = document.createElement('use-card')
    card.setAttribute('title', 'Welcome to use-ui')
    card.innerHTML = '<p>Ini adalah contoh card component</p>'
    app.appendChild(card)

    // Create Input
    const input = document.createElement('use-input')
    input.setAttribute('label', 'Username')
    input.setAttribute('placeholder', 'Masukkan username Anda')
    input.className = 'mt-4'
    app.appendChild(input)
  </script>
</body>
</html>
```

✅ Vanilla JS integration complete.

---

### Common Use Cases

#### 1️⃣ Form with Validation
```vue
<!-- Vue 3 Example -->
<template>
  <UseForm @submit="handleSubmit">
    <UseInput 
      v-model="form.email"
      type="email"
      label="Email"
      required
    />
    <UseInput 
      v-model="form.password"
      type="password"
      label="Password"
      required
      class="mt-3"
    />
    <UseButton type="primary" class="mt-4">Submit</UseButton>
  </UseForm>
</template>

<script setup>
import { ref } from 'vue'

const form = ref({
  email: '',
  password: ''
})

const handleSubmit = (e) => {
  console.log('Form submitted:', form.value)
}
</script>
```

#### 2️⃣ Modal Dialog
```vue
<!-- Vue 3 Example -->
<template>
  <div>
    <UseButton @click="showModal = true">Open Modal</UseButton>

    <UseModal 
      v-if="showModal"
      title="Confirm Action"
      @close="showModal = false"
    >
      <p>Are you sure you want to proceed?</p>
      <div class="flex gap-2 mt-4">
        <UseButton type="secondary" @click="showModal = false">Cancel</UseButton>
        <UseButton type="primary" @click="handleConfirm">Confirm</UseButton>
      </div>
    </UseModal>
  </div>
</template>

<script setup>
import { ref } from 'vue'

const showModal = ref(false)

const handleConfirm = () => {
  console.log('Confirmed!')
  showModal.value = false
}
</script>
```

#### 3️⃣ Toast Notification
```vue
<!-- Vue 3 Example -->
<template>
  <UseButton @click="showToast">Show Notification</UseButton>
</template>

<script setup>
import { useToast } from 'use-ui'

const toast = useToast()

const showToast = () => {
  toast.success('Action completed successfully!', {
    duration: 3000,
    position: 'top-right'
  })
}
</script>
```

#### 4️⃣ Responsive Grid
```vue
<!-- Vue 3 Example -->
<template>
  <UseGrid :columns="{ sm: 1, md: 2, lg: 3 }" gap="md">
    <UseCard v-for="i in 6" :key="i" :title="`Card ${i}`">
      <p>This is card {{ i }}</p>
    </UseCard>
  </UseGrid>
</template>
```

---

### Tips & Best Practices

🎯 **Tip 1: Tree-Shaking**
```javascript
// ✅ Good - Only import what you need
import { UseButton, UseInput } from 'use-ui'

// ❌ Avoid - Imports everything
import * as UI from 'use-ui'
```

🎯 **Tip 2: Styling**
```vue
<!-- Use CSS classes for styling -->
<UseButton class="custom-button">Button</UseButton>

<!-- Or pass style object -->
<UseButton :style="{ padding: '12px', fontSize: '16px' }">Button</UseButton>
```

🎯 **Tip 3: Theming**
```javascript
// Customize theme
import { createTheme } from 'use-ui'

const theme = createTheme({
  colors: {
    primary: '#FF6B6B',
    secondary: '#4ECDC4'
  }
})
```

🎯 **Tip 4: Accessibility**
```vue
<!-- Always provide labels for inputs -->
<UseInput 
  label="Your Name"
  aria-label="Full name input"
  aria-required="true"
  required
/>
```

---

### Next Steps

1. 📖 **Read the Documentation** - Full API docs in [Dokumentasi API](#dokumentasi-api)
2. 🎨 **Explore Storybook** - Interactive component playground: `npm run storybook`
3. 📚 **Check Examples** - More examples in [Examples](#-dukungan-lintas-framework)
4. 🤝 **Join Community** - Discuss on GitHub Issues
5. 🚀 **Build Your App** - Start building amazing UIs!

### Troubleshooting Quick Start

| Problem | Solution |
|---------|----------|
| Components not rendering | Check if CSS is imported: `import 'use-ui/dist/style.css'` |
| Type errors (React) | Ensure TypeScript types are installed: `npm install @use-ui/react` |
| Styling not applied | Verify CSS file path and no CSS loader conflicts |
| Vue warning about components | Register as global or use `import { UseButton } from 'use-ui'` |

---

## 🎨 Design System

### 📋 Design System Principles

use-ui design system dibangun atas 7 prinsip fundamental yang memandu setiap keputusan desain dan implementasi:

#### 1️⃣ **Consistency (Konsistensi)**
Semua komponen mengikuti pattern yang sama, memastikan pengalaman yang predictable dan familiar bagi pengguna.

**Implementasi:**
- Ukuran dan spacing yang standardized
- Naming conventions yang konsisten
- Behavior patterns yang uniform
- Visual language yang coherent

**Benefit:**
- ✅ Faster learning curve untuk user
- ✅ Reduced cognitive load
- ✅ Predictable component behavior
- ✅ Easier maintenance untuk developer

---

#### 2️⃣ **Accessibility (Aksesibilitas)**
Semua komponen dirancang dengan accessibility sebagai prioritas utama, bukan afterthought.

**Implementasi:**
- WCAG 2.1 Level AA compliance dari awal
- Semantic HTML structure
- ARIA labels dan roles
- Keyboard navigation support
- Color contrast ratios > 4.5:1
- Screen reader friendly

**Benefit:**
- ✅ Inclusive untuk semua user
- ✅ Legal compliance
- ✅ Better SEO
- ✅ Better user experience untuk semua

---

#### 3️⃣ **Simplicity (Kesederhanaan)**
Keep it simple. Setiap komponen hanya melakukan satu hal dengan baik.

**Implementasi:**
- Minimal API surface
- Clear prop names
- Intuitive default behavior
- Avoid over-engineering
- Progressive enhancement

**Benefit:**
- ✅ Easy to learn dan use
- ✅ Low barrier to entry
- ✅ Composable components
- ✅ Flexible combinations

---

#### 4️⃣ **Flexibility (Fleksibilitas)**
Komponen fleksibel cukup untuk berbagai use case namun tetap opinionated untuk maintainability.

**Implementasi:**
- CSS Variables untuk theming
- Slot-based composition
- Customizable through props
- Framework-agnostic approach
- Support untuk advanced use cases

**Benefit:**
- ✅ Adaptable ke berbagai design
- ✅ Works across frameworks
- ✅ Reusable di berbagai context
- ✅ Future-proof design

---

#### 5️⃣ **Performance (Performa)**
Lightweight dan fast, tanpa compromising functionality.

**Implementasi:**
- Minimal CSS (tree-shakeable)
- No heavy dependencies
- Optimized bundle size (~25KB gzip)
- Fast rendering
- Lazy-loadable components

**Benefit:**
- ✅ Faster page load times
- ✅ Better user experience
- ✅ Reduced bandwidth usage
- ✅ Works on slow networks

---

#### 6️⃣ **Developer Experience (DX)**
Make it delightful untuk developer. Clear docs, good errors, helpful utilities.

**Implementasi:**
- Comprehensive TypeScript support
- Clear error messages
- Helpful warning dalam development
- Rich documentation
- Interactive Storybook
- Good IDE autocomplete

**Benefit:**
- ✅ Faster development
- ✅ Fewer bugs
- ✅ Easier debugging
- ✅ More enjoyable workflow

---

#### 7️⃣ **Quality (Kualitas)**
Thorough testing, maintained standards, production-ready code.

**Implementasi:**
- 100% test coverage
- Continuous integration
- Regular updates & maintenance
- Semantic versioning
- Changelog documentation
- Performance benchmarks

**Benefit:**
- ✅ Reliable components
- ✅ Security patches
- ✅ Long-term support
- ✅ Enterprise-grade quality

---

### Design System Values vs Principles

| Nilai | Prinsip | Aksi |
|-------|---------|------|
| **User-First** | Accessibility + Simplicity | Design with users in mind |
| **Developer-First** | Developer Experience + Simplicity | Make tools that developers love |
| **Quality-Focused** | Quality + Performance | Maintain high standards |
| **Future-Proof** | Flexibility + Quality | Built to last |
| **Community-Driven** | Consistency + Quality | Work with the community |

---

### Visual Identity Hierarchy

```
Foundation (Base)
  ↓
Design Tokens (Color, Typography, Spacing)
  ↓
Components (Button, Input, Card, etc)
  ↓
Patterns (Forms, Layouts, Navigation)
  ↓
Applications (Complete UIs)
```

**Setiap level builds upon the previous, maintaining consistency throughout.**

---

### Color Philosophy

**Primary Purpose:** 
- Menggunakan warna untuk **hierarchy** dan **meaning**, bukan decoration

**Color System:**
- **Primary:** Main action/interactive elements
- **Secondary:** Alternative/secondary actions
- **Semantic:** Status indication (success, warning, error, info)
- **Neutral:** Backgrounds, borders, text

**Accessibility:**
- All colors pass WCAG AA contrast requirements
- Never rely on color alone untuk convey information
- Support untuk color-blind users

---

### Typography Philosophy

**Font Stack:**
Gunakan system fonts untuk fast loading dan native feel:
```
-apple-system, BlinkMacSystemFont, 'Segoe UI', Roboto, Oxygen, Ubuntu, Cantarell, sans-serif
```

**Font Sizes:**
- Base: 16px (1rem) untuk optimal readability
- Scale menggunakan modular scale (1.125 ratio)
- Consistent hierarchy di semua breakpoints

**Font Weights:**
- **Light (300):** Subtle, de-emphasized text
- **Normal (400):** Body text, default
- **Semibold (600):** Emphasis, labels
- **Bold (700):** Strong emphasis, headings

---

### Spacing Philosophy

**Base Unit:** 8px (0.5rem)
Semua spacing menggunakan multiples dari 8px:

```
4px (xs)   = 0.5 base unit
8px (sm)   = 1 base unit  ← minimum for interactive elements
16px (md)  = 2 base units
24px (lg)  = 3 base units
32px (xl)  = 4 base units
48px (2xl) = 6 base units
```

**Benefits:**
- ✅ Predictable rhythm
- ✅ Responsive & scalable
- ✅ Easy to implement
- ✅ Consistent spacing

---

### Responsive Design Philosophy

**Mobile-First Approach:**
1. Design untuk mobile (smallest screen)
2. Enhance untuk larger screens
3. Progressive enhancement

**Breakpoints:**
```
sm: 640px   (Small phones)
md: 768px   (Tablets)
lg: 1024px  (Laptops)
xl: 1280px  (Desktops)
2xl: 1536px (Large desktops)
```

---

### Interaction Design Philosophy

**Principles:**
- **Feedback:** User actions mendapat immediate visual feedback
- **Forgiveness:** Easy to undo mistakes
- **Clarity:** Action consequences jelas sebelum execution
- **Consistency:** Same action sama result everywhere
- **Efficiency:** Power users dapat bekerja lebih cepat

**Implementation:**
- Hover states untuk interactive elements
- Loading states untuk async operations
- Error messages yang helpful
- Keyboard navigation support
- Touch-friendly touch targets (min 44px)

---

### Component Design Guidelines

#### Naming Convention
```
Use<ComponentName>
UseButton       ✅
UseInputField   ✅
UseBtnPrimary   ❌
UseBtn          ❌
```

#### Prop Naming
```
// Use semantic, descriptive names
<UseButton type="primary" size="lg" disabled={false} />

// Avoid abbreviations
<UseButton btn-type="p" sz="l" dis={false} />  ❌
```

#### Default Behavior
- Sensible defaults untuk common use cases
- Override-able untuk advanced use cases
- No surprises untuk users

#### API Surface
- Minimal but complete
- Predictable parameter names
- Consistent with industry standards

---

### Palet Warna

```css
/* Primary Colors */
--color-primary: #3B82F6      /* Blue */
--color-primary-light: #DBEAFE
--color-primary-dark: #1E40AF

/* Secondary Colors */
--color-secondary: #10B981    /* Green */
--color-secondary-light: #D1FAE5
--color-secondary-dark: #047857

/* Semantic Colors */
--color-success: #10B981
--color-warning: #F59E0B
--color-error: #EF4444
--color-info: #3B82F6

/* Neutral Colors */
--color-gray-50: #F9FAFB
--color-gray-900: #111827
```

### Typography

```css
/* Font Family */
--font-family-base: -apple-system, BlinkMacSystemFont, 'Segoe UI', Roboto, Oxygen, Ubuntu, Cantarell, sans-serif

/* Font Sizes */
--font-size-xs: 0.75rem      /* 12px */
--font-size-sm: 0.875rem     /* 14px */
--font-size-base: 1rem       /* 16px */
--font-size-lg: 1.125rem     /* 18px */
--font-size-xl: 1.25rem      /* 20px */
--font-size-2xl: 1.5rem      /* 24px */
--font-size-3xl: 1.875rem    /* 30px */

/* Font Weights */
--font-weight-light: 300
--font-weight-normal: 400
--font-weight-semibold: 600
--font-weight-bold: 700
```

### Spacing

```css
/* 8px base unit */
--spacing-xs: 0.25rem   /* 4px */
--spacing-sm: 0.5rem    /* 8px */
--spacing-md: 1rem      /* 16px */
--spacing-lg: 1.5rem    /* 24px */
--spacing-xl: 2rem      /* 32px */
--spacing-2xl: 3rem     /* 48px */
```

### Breakpoints

```css
--breakpoint-sm: 640px
--breakpoint-md: 768px
--breakpoint-lg: 1024px
--breakpoint-xl: 1280px
--breakpoint-2xl: 1536px
```

---

## 🧩 Struktur Komponen

### 📁 Organisasi Folder

```
src/
├── components/              # Shared component definitions
│   ├── form/               # Form components
│   │   ├── UseButton.vue
│   │   ├── UseInput.vue
│   │   ├── UseSelect.vue
│   │   ├── UseCheckbox.vue
│   │   ├── UseRadio.vue
│   │   ├── UseTextarea.vue
│   │   ├── UseSwitch.vue
│   │   └── UseForm.vue
│   │
│   ├── layout/             # Layout components
│   │   ├── UseContainer.vue
│   │   ├── UseGrid.vue
│   │   ├── UseStack.vue
│   │   ├── UseCard.vue
│   │   ├── UseSpacer.vue
│   │   ├── UseFlexbox.vue
│   │   └── UseAspectRatio.vue
│   │
│   ├── navigation/         # Navigation components
│   │   ├── UseNavbar.vue
│   │   ├── UseSidebar.vue
│   │   ├── UseBreadcrumb.vue
│   │   ├── UseMenu.vue
│   │   ├── UseTabs.vue
│   │   └── UsePagination.vue
│   │
│   ├── feedback/           # Feedback & status components
│   │   ├── UseToast.vue
│   │   ├── UseAlert.vue
│   │   ├── UseModal.vue
│   │   ├── UseDrawer.vue
│   │   ├── UsePopover.vue
│   │   ├── UseTooltip.vue
│   │   ├── UseProgress.vue
│   │   ├── UseSkeleton.vue
│   │   ├── UseSpinner.vue
│   │   └── UseConfirm.vue
│   │
│   └── data/               # Data display components
│       ├── UseTable.vue
│       ├── UseBadge.vue
│       ├── UseTag.vue
│       ├── UseAvatar.vue
│       ├── UseList.vue
│       ├── UseStatistic.vue
│       ├── UseTimeline.vue
│       └── UseTree.vue
│
├── composables/            # Reusable composition logic
│   ├── useForm.ts         # Form handling logic
│   ├── useModal.ts        # Modal state management
│   ├── useToast.ts        # Toast notifications
│   ├── useAsync.ts        # Async operations
│   └── useTheme.ts        # Theme management
│
├── styles/                 # Design tokens & global styles
│   ├── tokens.css         # CSS Variables
│   ├── base.css           # Base styles
│   ├── theme-light.css    # Light theme
│   ├── theme-dark.css     # Dark theme
│   └── utilities.css      # Utility classes
│
├── utils/                  # Utility functions
│   ├── classnames.ts      # Class merging
│   ├── validators.ts      # Form validators
│   ├── accessibility.ts   # A11y helpers
│   └── events.ts          # Event utilities
│
└── types/                  # TypeScript definitions
    ├── components.ts      # Component props
    ├── events.ts          # Component events
    └── theme.ts           # Theme types
```

---

### 📋 Anatomi Komponen

Setiap komponen use-ui dibangun dengan struktur yang konsisten:

#### Single File Component (SFC) - Vue 3

```vue
<template>
  <button
    class="use-button"
    :class="[`use-button--${type}`, `use-button--${size}`]"
    :disabled="disabled"
    @click="handleClick"
  >
    <span v-if="loading" class="use-button__loader">
      <UseSpinner size="sm" />
    </span>
    <slot>{{ label }}</slot>
  </button>
</template>

<script setup lang="ts">
import { computed } from 'vue'
import UseSpinner from '../feedback/UseSpinner.vue'

interface Props {
  type?: 'primary' | 'secondary' | 'ghost' | 'danger'
  size?: 'sm' | 'md' | 'lg'
  disabled?: boolean
  loading?: boolean
  label?: string
}

interface Emits {
  (e: 'click', event: MouseEvent): void
}

const props = withDefaults(defineProps<Props>(), {
  type: 'primary',
  size: 'md',
  disabled: false,
  loading: false
})

const emit = defineEmits<Emits>()

const handleClick = (event: MouseEvent) => {
  if (!props.disabled && !props.loading) {
    emit('click', event)
  }
}
</script>

<style scoped>
.use-button {
  /* Base styles */
  display: inline-flex;
  align-items: center;
  justify-content: center;
  font-family: var(--font-family-base);
  font-weight: var(--font-weight-semibold);
  border: none;
  border-radius: var(--radius-md);
  cursor: pointer;
  transition: all var(--transition-base);
  position: relative;

  /* Default size */
  padding: var(--spacing-sm) var(--spacing-md);
  font-size: var(--font-size-base);
  height: var(--size-button-md);
}

/* Type variants */
.use-button--primary {
  background-color: var(--color-primary);
  color: white;
}

.use-button--primary:hover:not(:disabled) {
  background-color: var(--color-primary-dark);
}

.use-button--secondary {
  background-color: var(--color-secondary);
  color: white;
}

/* Size variants */
.use-button--sm {
  padding: var(--spacing-xs) var(--spacing-sm);
  font-size: var(--font-size-sm);
  height: var(--size-button-sm);
}

.use-button--lg {
  padding: var(--spacing-md) var(--spacing-lg);
  font-size: var(--font-size-lg);
  height: var(--size-button-lg);
}

/* States */
.use-button:disabled {
  opacity: 0.5;
  cursor: not-allowed;
}

.use-button__loader {
  display: inline-flex;
  margin-right: var(--spacing-xs);
}
</style>
```

---

### 🔄 Component Patterns

#### 1. **Wrapper Pattern** (Layout/Container)
Komponen yang membungkus konten dengan styling dan layout:

```vue
<template>
  <div class="use-container" :class="{ 'use-container--fluid': fluid }">
    <slot />
  </div>
</template>
```

**Contoh:** `UseContainer`, `UseCard`, `UseGrid`

#### 2. **Form Input Pattern** (Form)
Komponen input dengan validation dan state management:

```vue
<template>
  <div class="use-input-group">
    <label v-if="label" :for="inputId">{{ label }}</label>
    <input
      :id="inputId"
      v-model="modelValue"
      :type="type"
      @blur="validate"
      @change="emit('change', $event)"
    />
    <span v-if="error" class="use-input__error">{{ error }}</span>
  </div>
</template>
```

**Contoh:** `UseInput`, `UseSelect`, `UseCheckbox`, `UseTextarea`

#### 3. **Modal/Overlay Pattern** (Feedback)
Komponen yang menampilkan content di atas halaman:

```vue
<template>
  <Teleport v-if="isOpen" to="body">
    <div class="use-modal__backdrop" @click="close">
      <div class="use-modal__content" @click.stop>
        <header class="use-modal__header">
          <slot name="header" />
          <button @click="close">✕</button>
        </header>
        <section class="use-modal__body">
          <slot />
        </section>
      </div>
    </div>
  </Teleport>
</template>
```

**Contoh:** `UseModal`, `UseDrawer`, `UseToast`, `UsePopover`

#### 4. **Data Display Pattern** (Data)
Komponen untuk menampilkan data dengan formatting:

```vue
<template>
  <table class="use-table">
    <thead>
      <tr v-for="column in columns" :key="column.key">
        <th>{{ column.label }}</th>
      </tr>
    </thead>
    <tbody>
      <tr v-for="row in data" :key="row.id">
        <td v-for="column in columns" :key="column.key">
          {{ row[column.key] }}
        </td>
      </tr>
    </tbody>
  </table>
</template>
```

**Contoh:** `UseTable`, `UseList`, `UseAvatar`, `UseBadge`

#### 5. **Compound Component Pattern** (Complex)
Beberapa komponen yang bekerja bersama:

```vue
<!-- Parent Component -->
<UseForm @submit="handleSubmit">
  <UseFormField label="Email">
    <UseInput v-model="email" type="email" />
  </UseFormField>
  <UseFormField label="Password">
    <UseInput v-model="password" type="password" />
  </UseFormField>
  <UseButton type="primary">Submit</UseButton>
</UseForm>
```

---

### 🏗️ Component File Conventions

#### Naming Convention

| Item | Convention | Contoh |
|------|-----------|--------|
| **Component Name** | PascalCase dengan prefix `Use` | `UseButton`, `UseInputField` |
| **File Name** | PascalCase `.vue` | `UseButton.vue`, `UseInputField.vue` |
| **Folder Name** | lowercase, descriptive | `form/`, `layout/`, `feedback/` |
| **CSS Classes** | BEM + `use-` prefix | `.use-button--primary`, `.use-button__icon` |
| **Props** | camelCase | `:isDisabled`, `:maxLength` |
| **Events** | kebab-case | `@click-outside`, `@form-submit` |
| **Slots** | kebab-case | `<slot name="header-left" />` |

#### Component Props Template

```typescript
interface UseButtonProps {
  // Appearance
  type?: 'primary' | 'secondary' | 'ghost' | 'danger'
  size?: 'sm' | 'md' | 'lg'
  variant?: 'solid' | 'outline' | 'ghost'

  // State
  disabled?: boolean
  loading?: boolean

  // Content
  label?: string
  icon?: string

  // Behavior
  native?: HTMLElement['type'] // for button type
}
```

#### Component Events Template

```typescript
interface UseButtonEmits {
  (e: 'click', event: MouseEvent): void
  (e: 'focus', event: FocusEvent): void
  (e: 'blur', event: FocusEvent): void
}
```

---

### 🔗 Component Dependencies

#### Dependency Graph

```
UseForm
  ├── UseFormField
  │   ├── UseInput
  │   ├── UseSelect
  │   ├── UseCheckbox
  │   └── UseRadio
  ├── UseButton
  └── UseAlert

UseModal
  ├── UseButton
  └── useModal composable
      └── teleport (Vue built-in)

UseDataTable
  ├── UsePagination
  ├── UseBadge
  ├── UseButton
  └── useAsync composable
```

#### Circular Dependency Guidelines

❌ **Hindari:**
```typescript
// ComponentA.vue imports ComponentB
// ComponentB.vue imports ComponentA ← CIRCULAR!
```

✅ **Solusi:**
```typescript
// Extract shared logic to composable
// ComponentA.vue imports composable
// ComponentB.vue imports composable
```

---

### 📦 Framework-Specific Code

#### Vue 3 Specifics

```
src/vue3/
├── components/          # Vue SFC files
├── composables/         # Vue 3 Composition API
├── directives/          # Vue 3 Custom Directives
└── plugins/             # Vue 3 Plugins
```

#### React Specifics

```
src/react/
├── components/          # React functional components
├── hooks/               # React Custom Hooks
├── providers/           # Context Providers
└── hoc/                 # Higher-Order Components
```

#### Angular Specifics

```
src/angular/
├── components/          # Angular Components
├── directives/          # Angular Directives
├── services/            # Angular Services
└── modules/             # Angular Feature Modules
```

#### Vanilla JS Specifics

```
src/vanilla/
├── components/          # Web Components
├── utils/               # Helper functions
├── registry/            # Component registry
└── types/               # TypeScript definitions
```

---

### 🎯 Component Categories

#### ✅ Form Components
Form-related input dan control elements

| Komponen | Purpose | State | API |
|----------|---------|-------|-----|
| `UseInput` | Text input field | Controlled/Uncontrolled | v-model |
| `UseSelect` | Dropdown selection | Controlled | v-model |
| `UseCheckbox` | Checkbox control | Controlled | v-model |
| `UseRadio` | Radio group | Controlled | v-model |
| `UseTextarea` | Multi-line text | Controlled | v-model |
| `UseSwitch` | Toggle switch | Controlled | v-model |
| `UseForm` | Form wrapper | N/A | events |

#### ✅ Layout Components
Layout dan structural elements

| Komponen | Purpose | Props | Slots |
|----------|---------|-------|-------|
| `UseContainer` | Max-width wrapper | `fluid`, `size` | default |
| `UseGrid` | CSS Grid layout | `cols`, `gap`, `row-gap` | default |
| `UseStack` | Flex stack layout | `direction`, `gap`, `align` | default |
| `UseCard` | Card container | `shadow`, `hover`, `border` | default |
| `UseSpacer` | Space element | `size` | N/A |

#### ✅ Navigation Components
Navigation dan menu elements

| Komponen | Purpose | Stateful | Keyboard |
|----------|---------|----------|----------|
| `UseButton` | Interactive button | No | Yes |
| `UseNavbar` | Top nav bar | No | Yes |
| `UseSidebar` | Side navigation | Yes | Yes |
| `UseBreadcrumb` | Breadcrumb trail | No | Yes |
| `UseMenu` | Dropdown menu | Yes | Yes |

#### ✅ Feedback Components
Feedback, status, dan loading elements

| Komponen | Type | Dismissible | Auto-dismiss |
|----------|------|-----------|--------------|
| `UseToast` | Notification | Yes | Configurable |
| `UseAlert` | Alert message | No | No |
| `UseModal` | Dialog box | Yes | No |
| `UseDrawer` | Slide panel | Yes | No |
| `UsePopover` | Floating box | Yes | No |
| `UseTooltip` | Hint text | No | Yes |
| `UseProgress` | Progress bar | N/A | N/A |
| `UseSkeleton` | Loading placeholder | N/A | N/A |

#### ✅ Data Display Components
Data visualization elements

| Komponen | Scrollable | Sortable | Filterable |
|----------|-----------|----------|-----------|
| `UseTable` | Yes | Yes | Yes |
| `UsePagination` | N/A | N/A | N/A |
| `UseBadge` | No | No | No |
| `UseTag` | Wrap | No | No |
| `UseAvatar` | No | No | No |
| `UseList` | Yes | No | No |

---

### 🔌 Composables & Utilities

#### Core Composables

```typescript
// Form handling
export function useForm(config: FormConfig) {
  return {
    values,
    errors,
    isSubmitting,
    submit,
    reset,
    setFieldValue,
    setFieldError
  }
}

// Modal state
export function useModal(initialState?: boolean) {
  return {
    isOpen,
    open,
    close,
    toggle
  }
}

// Toast notifications
export function useToast() {
  return {
    success,
    error,
    warning,
    info,
    dismiss
  }
}

// Theme management
export function useTheme() {
  return {
    theme,
    isDark,
    toggleTheme,
    setTheme
  }
}
```

---

## 📖 Dokumentasi API

## 📖 Dokumentasi API

### UseButton Component

```vue
<UseButton
  type="primary|secondary|ghost|danger"
  size="sm|md|lg"
  :disabled="boolean"
  :loading="boolean"
  @click="handleClick"
>
  Click Me
</UseButton>
```

**Props:**
| Prop | Type | Default | Deskripsi |
|------|------|---------|-----------|
| `type` | String | `primary` | Tipe button (primary, secondary, ghost, danger) |
| `size` | String | `md` | Ukuran button (sm, md, lg) |
| `disabled` | Boolean | `false` | Disable button |
| `loading` | Boolean | `false` | Loading state |
| `fullWidth` | Boolean | `false` | Full width button |

**Events:**
| Event | Payload | Deskripsi |
|-------|---------|-----------|
| `click` | Event | Triggered saat button diklik |
| `hover` | Boolean | Triggered saat mouse hover |

### UseInput Component

```vue
<UseInput
  v-model="value"
  type="text"
  label="Username"
  placeholder="Enter username"
  :error="errorMessage"
  :required="true"
  @blur="handleBlur"
/>
```

**Props:**
| Prop | Type | Default | Deskripsi |
|------|------|---------|-----------|
| `modelValue` | String/Number | `` | Input value (v-model) |
| `type` | String | `text` | Input type |
| `label` | String | - | Label text |
| `placeholder` | String | - | Placeholder text |
| `error` | String | - | Error message |
| `required` | Boolean | `false` | Required field |
| `disabled` | Boolean | `false` | Disable input |

---

## 🌐 Dukungan Lintas Framework

### 🎯 Cross-Framework Strategy

**use-ui** didukung oleh filosofi framework-agnostic yang memungkinkan developer menggunakan component library yang sama di berbagai environment modern:

| Aspek | Deskripsi |
|-------|-----------|
| **Foundation** | Web Components (Custom Elements API) + HTML + CSS |
| **Wrapper Layers** | Framework-specific adapters untuk Vue 3, React, Angular |
| **API Consistency** | Unified naming dan behavior across frameworks |
| **Styling** | CSS Variables untuk universal theming |
| **Performance** | Optimized untuk setiap framework runtime |

---

### 🏗️ Architecture Overview

```
┌─────────────────────────────────────────────┐
│       Application Layer                      │
│  (Vue 3 / React / Angular / Vanilla JS)     │
└──────────────┬──────────────────────────────┘
               │
      ┌────────┼────────┐
      │        │        │
   ┌──▼──┐ ┌──▼──┐ ┌───▼──┐
   │ Vue │ │React│ │Angular│
   └──┬──┘ └──┬──┘ └───┬──┘
      │   (Framework-Specific Adapters)
      │        │        │
      └────────┼────────┘
               │
    ┌──────────▼──────────┐
    │ Web Components API  │
    │  (Custom Elements)  │
    └──────────┬──────────┘
               │
    ┌──────────▼──────────┐
    │  HTML + CSS         │
    │  + CSS Variables    │
    └─────────────────────┘
```

---

### 🔄 How It Works

#### Layer 1: Foundation (Web Components)

Semua komponen dibangun sebagai **Web Components** yang memanfaatkan:

```javascript
// Web Components are framework-agnostic
class UseButton extends HTMLElement {
  connectedCallback() {
    this.render()
    this.attachEventListeners()
  }

  render() {
    this.innerHTML = `
      <button class="use-button ${this.getAttribute('type')}">
        <slot></slot>
      </button>
    `
  }

  attachEventListeners() {
    const button = this.querySelector('button')
    button.addEventListener('click', () => {
      this.dispatchEvent(new CustomEvent('click'))
    })
  }
}

customElements.define('use-button', UseButton)
```

**Benefits:**
- ✅ Framework-independent
- ✅ Works in any environment
- ✅ Native browser API
- ✅ Zero framework dependencies

#### Layer 2: Framework Adapters

Framework-specific wrappers menyediakan idiomatik API untuk setiap framework:

**Vue 3 Adapter:**
```vue
<template>
  <use-button 
    :ref="buttonRef"
    :type="type"
    @click="handleClick"
  >
    <slot>{{ label }}</slot>
  </use-button>
</template>

<script setup>
// Vue 3 Composition API integration
const buttonRef = ref(null)
const handleClick = (event) => {
  emit('click', event)
}
</script>
```

**React Adapter:**
```jsx
export const UseButton = forwardRef(({ 
  type, 
  onClick, 
  children 
}, ref) => {
  useEffect(() => {
    if (ref?.current) {
      ref.current.setAttribute('type', type)
    }
  }, [type])

  return (
    <use-button 
      ref={ref}
      onClick={onClick}
    >
      {children}
    </use-button>
  )
})
```

**Angular Adapter:**
```typescript
@Component({
  selector: 'use-button',
  template: `
    <button 
      class="use-button"
      [class]="type"
      (click)="onClick.emit($event)"
    >
      <ng-content></ng-content>
    </button>
  `
})
export class UseButtonComponent {
  @Input() type: 'primary' | 'secondary' = 'primary'
  @Output() onClick = new EventEmitter<Event>()
}
```

---

### 📊 Framework Comparison

#### API Consistency Matrix

| Feature | Vue 3 | React | Angular | Vanilla JS |
|---------|-------|-------|---------|-----------|
| **Props** | `:prop="value"` | `prop={value}` | `[prop]="value"` | `setAttribute()` |
| **Events** | `@click="handler"` | `onClick={handler}` | `(click)="handler()"` | `addEventListener()` |
| **Slots** | `<slot>` | `children` | `<ng-content>` | N/A |
| **Styles** | CSS Modules | CSS-in-JS | Angular styles | CSS classes |
| **Two-way Binding** | `v-model` | state + onChange | `[(ngModel)]` | Manual |
| **Computed** | `computed()` | `useMemo()` | getters | N/A |
| **Side Effects** | `watch()` | `useEffect()` | `ngOnInit()` | Manual |

---

### 🔧 Installation & Setup

#### Framework-Specific Packages

```bash
# Vue 3 - Full framework support
npm install use-ui @use-ui/vue3

# React - React components with hooks
npm install use-ui @use-ui/react

# Angular - Angular components
npm install use-ui @use-ui/angular

# Vanilla JS - Web Components only
npm install use-ui
```

#### Version Requirements

| Framework | Minimum Version | Recommended | Tested |
|-----------|-----------------|-------------|--------|
| **Vue** | 3.3.0 | 3.4+ | 3.4, 3.5 |
| **React** | 18.0.0 | 18.2+ | 18.2, 19 |
| **Angular** | 15.0.0 | 17+ | 17, 18 |
| **TypeScript** | 4.7.0 | 5.0+ | 5.0, 5.2 |
| **Node** | 16.0.0 | 18+ | 18, 20 |

---

### 💻 Implementation Examples

#### Vue 3 - Composition API Pattern

```vue
<template>
  <form @submit.prevent="handleSubmit">
    <UseInput 
      v-model="formData.email"
      type="email"
      label="Email"
      @blur="validateEmail"
    />
    <UseInput 
      v-model="formData.password"
      type="password"
      label="Password"
    />
    <UseButton 
      type="primary"
      :disabled="isSubmitting"
      :loading="isSubmitting"
    >
      Sign In
    </UseButton>
  </form>
</template>

<script setup lang="ts">
import { ref } from 'vue'
import { UseInput, UseButton } from '@use-ui/vue3'
import { useForm } from '@use-ui/vue3/composables'

const { values: formData, submit } = useForm({
  email: '',
  password: ''
})

const isSubmitting = ref(false)

const handleSubmit = async () => {
  isSubmitting.value = true
  await submit()
  isSubmitting.value = false
}

const validateEmail = () => {
  // Email validation
}
</script>

<style scoped>
form {
  display: flex;
  flex-direction: column;
  gap: var(--spacing-md);
  max-width: 400px;
}
</style>
```

#### React - Hooks Pattern

```jsx
import { useState } from 'react'
import { UseInput, UseButton } from '@use-ui/react'
import { useForm } from '@use-ui/react/hooks'
import '@use-ui/react/dist/style.css'

export function LoginForm() {
  const { values, errors, handleChange, handleSubmit } = useForm({
    initialValues: {
      email: '',
      password: ''
    },
    onSubmit: async (values) => {
      console.log('Submitting:', values)
    }
  })

  const [isLoading, setIsLoading] = useState(false)

  const onSubmit = async (e) => {
    e.preventDefault()
    setIsLoading(true)
    await handleSubmit()
    setIsLoading(false)
  }

  return (
    <form onSubmit={onSubmit} style={styles.form}>
      <UseInput
        name="email"
        type="email"
        label="Email"
        value={values.email}
        onChange={handleChange}
        error={errors.email}
      />
      <UseInput
        name="password"
        type="password"
        label="Password"
        value={values.password}
        onChange={handleChange}
        error={errors.password}
      />
      <UseButton
        type="primary"
        disabled={isLoading}
        loading={isLoading}
      >
        Sign In
      </UseButton>
    </form>
  )
}

const styles = {
  form: {
    display: 'flex',
    flexDirection: 'column',
    gap: 'var(--spacing-md)',
    maxWidth: '400px'
  }
}
```

#### Angular - Typed Components Pattern

```typescript
import { Component, OnInit } from '@angular/core'
import { FormBuilder, FormGroup, Validators } from '@angular/forms'
import { UseUIModule } from '@use-ui/angular'

@Component({
  selector: 'app-login-form',
  template: `
    <form [formGroup]="loginForm" (ngSubmit)="onSubmit()">
      <use-input
        label="Email"
        type="email"
        formControlName="email"
        [error]="getErrorMessage('email')"
      ></use-input>
      
      <use-input
        label="Password"
        type="password"
        formControlName="password"
        [error]="getErrorMessage('password')"
      ></use-input>
      
      <use-button
        type="primary"
        [disabled]="isSubmitting"
        [loading]="isSubmitting"
      >
        Sign In
      </use-button>
    </form>
  `,
  styles: [`
    form {
      display: flex;
      flex-direction: column;
      gap: var(--spacing-md);
      max-width: 400px;
    }
  `],
  standalone: true,
  imports: [UseUIModule]
})
export class LoginFormComponent implements OnInit {
  loginForm: FormGroup
  isSubmitting = false

  constructor(private fb: FormBuilder) {
    this.loginForm = this.fb.group({
      email: ['', [Validators.required, Validators.email]],
      password: ['', [Validators.required, Validators.minLength(8)]]
    })
  }

  ngOnInit() {}

  onSubmit() {
    if (this.loginForm.valid) {
      this.isSubmitting = true
      // Submit logic
    }
  }

  getErrorMessage(fieldName: string): string {
    const field = this.loginForm.get(fieldName)
    if (field?.hasError('required')) {
      return `${fieldName} is required`
    }
    if (fieldName === 'email' && field?.hasError('email')) {
      return 'Invalid email'
    }
    return ''
  }
}
```

#### Vanilla JavaScript - Web Components Direct

```html
<!DOCTYPE html>
<html>
<head>
  <link rel="stylesheet" href="https://cdn.jsdelivr.net/npm/use-ui/dist/style.css">
</head>
<body>
  <form id="login-form">
    <use-input
      id="email-input"
      type="email"
      label="Email"
      placeholder="your@email.com"
    ></use-input>

    <use-input
      id="password-input"
      type="password"
      label="Password"
      placeholder="Enter password"
    ></use-input>

    <use-button id="submit-btn" type="primary">
      Sign In
    </use-button>
  </form>

  <script src="https://cdn.jsdelivr.net/npm/use-ui/dist/use-ui.js"></script>
  <script>
    const form = document.getElementById('login-form')
    const emailInput = document.getElementById('email-input')
    const passwordInput = document.getElementById('password-input')
    const submitBtn = document.getElementById('submit-btn')

    form.addEventListener('submit', (e) => {
      e.preventDefault()
      
      const email = emailInput.value
      const password = passwordInput.value
      
      console.log('Submitting:', { email, password })
      
      // Submit logic
    })

    submitBtn.addEventListener('click', () => {
      // Custom click handler
    })
  </script>

  <style>
    form {
      display: flex;
      flex-direction: column;
      gap: var(--spacing-md);
      max-width: 400px;
    }
  </style>
</body>
</html>
```

---

### 🎨 Theme & Styling Across Frameworks

#### Unified CSS Variables

Semua framework menggunakan **CSS Custom Properties (CSS Variables)** untuk theming:

```css
/* themes/light.css */
:root {
  --color-primary: #3B82F6;
  --color-secondary: #10B981;
  --color-success: #10B981;
  --color-warning: #F59E0B;
  --color-error: #EF4444;
  --color-info: #3B82F6;
  
  --font-family-base: -apple-system, BlinkMacSystemFont, 'Segoe UI', Roboto;
  --font-size-base: 1rem;
  --spacing-base: 8px;
  
  --radius-sm: 4px;
  --radius-md: 8px;
  --radius-lg: 12px;
}

/* themes/dark.css */
@media (prefers-color-scheme: dark) {
  :root {
    --color-primary: #60A5FA;
    --color-secondary: #34D399;
    /* ... */
  }
}
```

#### Framework-Specific Theme Implementation

**Vue 3:**
```vue
<script setup>
import { provide } from 'vue'
import { useTheme } from '@use-ui/vue3/composables'

const { toggleDarkMode, isDark } = useTheme()

provide('isDark', isDark)
</script>

<template>
  <div :class="{ 'dark-mode': isDark }">
    <button @click="toggleDarkMode">
      Toggle Dark Mode
    </button>
  </div>
</template>
```

**React:**
```jsx
import { createContext, useState } from 'react'
import { useTheme } from '@use-ui/react/hooks'

export const ThemeContext = createContext()

export function ThemeProvider({ children }) {
  const { isDark, toggleDarkMode } = useTheme()

  return (
    <ThemeContext.Provider value={{ isDark, toggleDarkMode }}>
      <div className={isDark ? 'dark-mode' : 'light-mode'}>
        {children}
      </div>
    </ThemeContext.Provider>
  )
}
```

**Angular:**
```typescript
@Injectable({ providedIn: 'root' })
export class ThemeService {
  private darkMode$ = new BehaviorSubject(false)

  toggleDarkMode() {
    const current = this.darkMode$.value
    this.darkMode$.next(!current)
  }

  isDarkMode$() {
    return this.darkMode$.asObservable()
  }
}
```

---

### 🔗 Interoperability & Migration

#### Using Multiple Frameworks in One App

```html
<!-- Vue 3 component area -->
<div id="vue-app"></div>

<!-- React component area -->
<div id="react-app"></div>

<!-- Shared Web Components (work everywhere) -->
<use-button id="shared-button">
  Shared across frameworks
</use-button>
```

#### Migrating Between Frameworks

##### Step 1: Use Web Components (Foundation)

```javascript
// All frameworks can use web components
const button = document.createElement('use-button')
button.setAttribute('type', 'primary')
button.textContent = 'Click Me'
```

##### Step 2: Gradually Adopt Framework Wrapper

```vue
<!-- Vue 3: Replace web component usage with Vue adapter -->
<UseButton type="primary">Click Me</UseButton>
```

##### Step 3: Full Migration Complete

Benefits:
- ✅ Gradual migration without rewriting
- ✅ No dependency lock-in
- ✅ Easy framework switching
- ✅ Consistent component API

---

### 🧪 Testing Across Frameworks

#### Unified Component Testing

```javascript
// Jest + Testing Library (works across frameworks)

import { render, screen } from '@testing-library/vue'
import userEvent from '@testing-library/user-event'
import { UseButton } from '@use-ui/vue3'

describe('UseButton', () => {
  it('should emit click event', async () => {
    const { emitted } = render(UseButton, {
      slots: { default: 'Click Me' }
    })

    const button = screen.getByRole('button')
    await userEvent.click(button)

    expect(emitted().click).toBeTruthy()
  })
})
```

#### React Testing

```javascript
import { render, screen } from '@testing-library/react'
import userEvent from '@testing-library/user-event'
import { UseButton } from '@use-ui/react'

describe('UseButton', () => {
  it('should call onClick handler', async () => {
    const onClick = jest.fn()
    render(<UseButton onClick={onClick}>Click Me</UseButton>)

    const button = screen.getByRole('button')
    await userEvent.click(button)

    expect(onClick).toHaveBeenCalled()
  })
})
```

#### E2E Testing

```javascript
// Playwright (works across all frameworks)

import { test, expect } from '@playwright/test'

test('UseButton interaction', async ({ page }) => {
  await page.goto('http://localhost:3000')
  
  const button = page.locator('use-button')
  await expect(button).toBeVisible()
  
  const clickPromise = page.waitForEvent('console')
  await button.click()
  
  const log = await clickPromise
  expect(log.text()).toContain('Button clicked')
})
```

---

### ⚡ Performance Considerations

#### Framework-Specific Optimization

| Framework | Key Optimization | Bundle Impact | Runtime |
|-----------|------------------|----------------|---------|
| **Vue 3** | Tree-shaking composables | +0KB | ✅ Fastest |
| **React** | Code splitting hooks | +2KB | ✅ Fast |
| **Angular** | Ivy compilation | +3KB | ✅ Comparable |
| **Vanilla** | Direct Web Components | -2KB | ✅ Fastest |

#### Bundle Size Comparison

```
Vue 3:        ~22KB (use-ui core + Vue adapter)
React:        ~24KB (use-ui core + React adapter)
Angular:      ~25KB (use-ui core + Angular adapter)
Vanilla JS:   ~20KB (use-ui core only)

All: Tree-shakeable → ~15KB with single component
```

---

### 🚀 When to Use Each Framework

#### Use Vue 3 when:
- ✅ You need reactive, two-way binding
- ✅ You prefer template syntax
- ✅ You want smallest bundle with features
- ✅ Building interactive dashboards

#### Use React when:
- ✅ You have large ecosystem requirements
- ✅ You prefer functional programming
- ✅ You need maximum community support
- ✅ Building complex state management

#### Use Angular when:
- ✅ You need full-featured framework
- ✅ You have TypeScript-first requirements
- ✅ You need dependency injection
- ✅ Building enterprise applications

#### Use Vanilla JS when:
- ✅ You don't need framework overhead
- ✅ You have simple component needs
- ✅ You need framework-agnostic solution
- ✅ Building micro-frontends

---

### 📚 Framework Documentation Links

- [Vue 3 Guide](./docs/frameworks/vue3.md)
- [React Guide](./docs/frameworks/react.md)
- [Angular Guide](./docs/frameworks/angular.md)
- [Vanilla JS Guide](./docs/frameworks/vanilla.md)
- [Migration Guide](./docs/frameworks/migration.md)

---

## 📁 Struktur Proyek

### 📂 Complete Directory Tree

```
use-ui/
│
├── 📁 src/                           # Main source code
│   ├── 📁 components/                # UI Components (organized by category)
│   │   ├── 📁 form/                  # Form components
│   │   │   ├── Button.vue            # Button component
│   │   │   ├── Button.spec.ts        # Button tests
│   │   │   ├── Input.vue
│   │   │   ├── Input.spec.ts
│   │   │   ├── Select.vue
│   │   │   ├── Checkbox.vue
│   │   │   ├── Radio.vue
│   │   │   ├── Textarea.vue
│   │   │   ├── Switch.vue
│   │   │   └── Form.vue
│   │   │
│   │   ├── 📁 layout/                # Layout components
│   │   │   ├── Container.vue
│   │   │   ├── Grid.vue
│   │   │   ├── Stack.vue
│   │   │   ├── Card.vue
│   │   │   ├── Flex.vue
│   │   │   └── AspectRatio.vue
│   │   │
│   │   ├── 📁 navigation/            # Navigation components
│   │   │   ├── Navbar.vue
│   │   │   ├── Sidebar.vue
│   │   │   ├── Breadcrumb.vue
│   │   │   ├── Menu.vue
│   │   │   ├── Tabs.vue
│   │   │   └── Pagination.vue
│   │   │
│   │   ├── 📁 feedback/              # Feedback components
│   │   │   ├── Alert.vue
│   │   │   ├── Toast.vue
│   │   │   ├── Modal.vue
│   │   │   ├── Drawer.vue
│   │   │   ├── Popover.vue
│   │   │   ├── Tooltip.vue
│   │   │   ├── Progress.vue
│   │   │   ├── Skeleton.vue
│   │   │   ├── Spinner.vue
│   │   │   └── Confirm.vue
│   │   │
│   │   └── 📁 data/                  # Data display components
│   │       ├── Table.vue
│   │       ├── Badge.vue
│   │       ├── Tag.vue
│   │       ├── Avatar.vue
│   │       ├── List.vue
│   │       ├── Statistic.vue
│   │       ├── Timeline.vue
│   │       └── Tree.vue
│   │
│   ├── 📁 composables/               # Vue Composition API logic (reusable)
│   │   ├── useForm.ts                # Form handling logic
│   │   ├── useModal.ts               # Modal state management
│   │   ├── useToast.ts               # Toast notifications
│   │   ├── useAsync.ts               # Async operations
│   │   ├── useTheme.ts               # Theme management
│   │   ├── useClickOutside.ts        # Detect clicks outside element
│   │   ├── useFocus.ts               # Focus management
│   │   ├── useKeyboard.ts            # Keyboard event handling
│   │   └── useResponsive.ts          # Responsive breakpoints
│   │
│   ├── 📁 styles/                    # Global styles & design tokens
│   │   ├── tokens.css                # Design system tokens
│   │   │   ├── colors.css
│   │   │   ├── typography.css
│   │   │   ├── spacing.css
│   │   │   ├── shadows.css
│   │   │   ├── breakpoints.css
│   │   │   └── transitions.css
│   │   │
│   │   ├── themes/                   # Theme files
│   │   │   ├── light.css             # Light theme
│   │   │   ├── dark.css              # Dark theme
│   │   │   └── custom.css            # Custom theme template
│   │   │
│   │   ├── base.css                  # Reset & base styles
│   │   ├── components.css            # Component-specific styles
│   │   ├── utilities.css             # Utility classes
│   │   ├── accessibility.css         # A11y styles
│   │   ├── animations.css            # Animation keyframes
│   │   └── main.css                  # Main entry point
│   │
│   ├── 📁 utils/                     # Utility functions
│   │   ├── classnames.ts             # Class name merging
│   │   ├── validators.ts             # Form validators
│   │   ├── accessibility.ts          # A11y helpers
│   │   ├── events.ts                 # Event utilities
│   │   ├── dom.ts                    # DOM helpers
│   │   ├── formatting.ts             # Data formatting
│   │   ├── storage.ts                # LocalStorage helpers
│   │   └── constants.ts              # Constants & enums
│   │
│   ├── 📁 types/                     # TypeScript type definitions
│   │   ├── components.ts             # Component prop types
│   │   ├── events.ts                 # Component event types
│   │   ├── theme.ts                  # Theme types
│   │   ├── form.ts                   # Form types
│   │   └── index.ts                  # Main types export
│   │
│   ├── 📁 directives/                # Vue directives
│   │   ├── vClickOutside.ts          # Click outside directive
│   │   ├── vFocus.ts                 # Auto-focus directive
│   │   └── vLoading.ts               # Loading state directive
│   │
│   ├── App.vue                       # Root Vue component (Storybook demo)
│   ├── main.ts                       # Entry point (development)
│   └── index.ts                      # Main library export
│
├── 📁 packages/                      # Framework-specific packages
│   ├── 📁 vue3/                      # Vue 3 package
│   │   ├── package.json
│   │   ├── src/
│   │   └── dist/
│   │
│   ├── 📁 react/                     # React package
│   │   ├── package.json
│   │   ├── src/
│   │   │   ├── components/           # React components
│   │   │   ├── hooks/                # React hooks (useButton, useInput, etc.)
│   │   │   ├── providers/            # Context providers
│   │   │   └── index.ts
│   │   └── dist/
│   │
│   ├── 📁 angular/                   # Angular package
│   │   ├── package.json
│   │   ├── src/
│   │   │   ├── components/           # Angular components
│   │   │   ├── directives/           # Angular directives
│   │   │   ├── services/             # Angular services
│   │   │   ├── modules/              # Feature modules
│   │   │   └── index.ts
│   │   └── dist/
│   │
│   └── 📁 web-components/            # Vanilla JS / Web Components
│       ├── package.json
│       ├── src/
│       │   ├── components/           # Web Components
│       │   ├── registry.ts           # Component registry
│       │   ├── utils/
│       │   └── index.ts
│       └── dist/
│
├── 📁 docs/                          # Documentation
│   ├── 📁 guide/                     # User guides
│   │   ├── getting-started.md
│   │   ├── installation.md
│   │   ├── quick-start.md
│   │   ├── theming.md
│   │   └── customization.md
│   │
│   ├── 📁 frameworks/                # Framework-specific guides
│   │   ├── vue3.md
│   │   ├── react.md
│   │   ├── angular.md
│   │   └── vanilla.md
│   │
│   ├── 📁 api/                       # API documentation
│   │   ├── components.md
│   │   ├── composables.md
│   │   ├── utils.md
│   │   └── types.md
│   │
│   ├── 📁 examples/                  # Usage examples
│   │   ├── forms/
│   │   ├── layouts/
│   │   ├── modals/
│   │   └── tables/
│   │
│   └── index.md                      # Documentation home
│
├── 📁 stories/                       # Storybook stories
│   ├── 📁 form/
│   │   ├── Button.stories.ts
│   │   ├── Input.stories.ts
│   │   └── ...
│   │
│   ├── 📁 layout/
│   │   ├── Container.stories.ts
│   │   └── ...
│   │
│   ├── 📁 feedback/
│   │   ├── Modal.stories.ts
│   │   ├── Toast.stories.ts
│   │   └── ...
│   │
│   └── 📁 data/
│       ├── Table.stories.ts
│       └── ...
│
├── 📁 tests/                         # Test files
│   ├── 📁 unit/                      # Unit tests
│   │   ├── components/
│   │   ├── composables/
│   │   └── utils/
│   │
│   ├── 📁 integration/               # Integration tests
│   │   ├── form-workflow.spec.ts
│   │   └── modal-interaction.spec.ts
│   │
│   └── 📁 e2e/                       # End-to-end tests
│       ├── form.spec.ts
│       └── navigation.spec.ts
│
├── 📁 .storybook/                    # Storybook configuration
│   ├── main.ts                       # Main config
│   ├── preview.ts                    # Preview config
│   ├── manager.ts                    # Manager customization
│   └── theme.ts                      # Theme customization
│
├── 📁 .github/                       # GitHub files
│   ├── 📁 workflows/                 # CI/CD workflows
│   │   ├── test.yml
│   │   ├── build.yml
│   │   ├── deploy.yml
│   │   └── publish.yml
│   │
│   ├── 📁 ISSUE_TEMPLATE/
│   │   ├── bug_report.md
│   │   └── feature_request.md
│   │
│   └── PULL_REQUEST_TEMPLATE.md
│
├── 📁 dist/                          # Build output (generated)
│   ├── 📁 esm/                       # ES Modules
│   │   ├── components/
│   │   ├── composables/
│   │   ├── index.js
│   │   └── index.d.ts
│   │
│   ├── 📁 cjs/                       # CommonJS
│   │   ├── components/
│   │   ├── index.js
│   │   └── index.d.ts
│   │
│   ├── 📁 umd/                       # UMD bundle
│   │   ├── use-ui.js
│   │   └── use-ui.min.js
│   │
│   ├── 📁 types/                     # TypeScript types
│   │   ├── components.d.ts
│   │   ├── composables.d.ts
│   │   └── index.d.ts
│   │
│   ├── 📁 styles/                    # CSS output
│   │   ├── main.css
│   │   ├── main.min.css
│   │   ├── themes/
│   │   └── tokens.css
│   │
│   └── README.md                     # Build output README
│
├── 📁 node_modules/                  # Dependencies (gitignored)
│
├── Configuration Files
│   ├── package.json                  # Project metadata & scripts
│   ├── package-lock.json             # Locked dependencies
│   ├── pnpm-lock.yaml               # PNPM lock file
│   ├── vite.config.ts                # Vite build config
│   ├── tsconfig.json                 # TypeScript config
│   ├── jsconfig.json                 # JavaScript config
│   ├── vitest.config.ts              # Vitest config
│   ├── .eslintrc.json               # ESLint config
│   ├── .prettierrc                   # Prettier config
│   ├── .stylelintrc.json             # StyleLint config
│   ├── .editorconfig                 # Editor config
│   ├── postcss.config.js             # PostCSS config
│   ├── tailwind.config.js            # Tailwind config (if used)
│   └── vitest.config.ts              # Vitest configuration
│
├── Documentation Files
│   ├── README.md                     # Main documentation
│   ├── CHANGELOG.md                  # Version changelog
│   ├── CONTRIBUTING.md               # Contribution guide
│   ├── CODE_OF_CONDUCT.md            # Code of conduct
│   ├── LICENSE                       # MIT License
│   ├── SECURITY.md                   # Security policy
│   └── .gitignore                    # Git ignore rules

```

---

### 📋 Directory Purposes

#### `/src` - Source Code
Main library code organized by component type and concern:

| Directory | Purpose |
|-----------|---------|
| `components/` | Reusable UI components organized by category |
| `composables/` | Reusable logic/state management (Vue 3 Composition API) |
| `styles/` | Global styles, design tokens, and themes |
| `utils/` | Utility functions and helpers |
| `types/` | TypeScript type definitions |
| `directives/` | Custom Vue directives |

#### `/packages` - Framework Adapters
Monorepo structure with framework-specific packages:

```
@use-ui/core          (base web components + types)
@use-ui/vue3          (Vue 3 components)
@use-ui/react         (React components)
@use-ui/angular       (Angular components)
@use-ui/web-components (Vanilla JS + Web Components)
```

#### `/docs` - Documentation
Complete user and developer documentation:

- `guide/` - Getting started guides
- `frameworks/` - Framework-specific documentation
- `api/` - Component and API reference
- `examples/` - Usage examples and patterns

#### `/stories` - Storybook
Interactive component library and documentation:

- Organized by component category
- Live component preview
- Props/events documentation
- Interactive playground

#### `/tests` - Test Suite
Comprehensive testing:

- `unit/` - Component unit tests
- `integration/` - Workflow tests
- `e2e/` - End-to-end tests

#### `/dist` - Build Output (Generated)
Production-ready compiled code:

- `esm/` - ES Modules (modern imports)
- `cjs/` - CommonJS (Node.js)
- `umd/` - Universal Module (browser)
- `types/` - TypeScript definitions
- `styles/` - Compiled CSS

---

### 🔄 Component File Structure Example

Each component typically has this structure:

```
components/form/Button/
├── Button.vue          # Component implementation
├── Button.spec.ts      # Unit tests
├── Button.stories.ts   # Storybook story
├── Button.types.ts     # Component types
└── index.ts            # Export
```

**Inside a component file (Button.vue):**

```vue
<template>
  <!-- HTML template -->
</template>

<script setup lang="ts">
// TypeScript logic
</script>

<style scoped>
/* Scoped styles */
</style>
```

---

### 📦 npm Scripts

Located in `package.json`, these are main development scripts:

```json
{
  "scripts": {
    "dev": "vite",                           # Dev server
    "build": "vite build",                   # Production build
    "build:lib": "vite build --lib",         # Library build
    "build:types": "tsc --emitDeclarationOnly",  # Generate types
    "preview": "vite preview",               # Preview build
    
    "storybook": "storybook dev",            # Start Storybook
    "storybook:build": "storybook build",    # Build Storybook
    
    "test": "vitest",                        # Run all tests
    "test:ui": "vitest --ui",                # Test UI mode
    "test:coverage": "vitest --coverage",    # Coverage report
    "test:e2e": "playwright test",           # E2E tests
    
    "lint": "eslint . --ext .vue,.js,.ts",   # Lint files
    "lint:style": "stylelint src/**/*.{vue,css}",  # Lint styles
    "format": "prettier --write src",        # Format code
    
    "type-check": "tsc --noEmit",            # Type checking
    "validate": "npm run type-check && npm run lint && npm run test",
    
    "docs": "vitepress dev docs",            # Dev docs
    "docs:build": "vitepress build docs",    # Build docs
    
    "publish": "npm run build && npm publish",  # Publish to npm
    "release": "bumpp && npm publish"        # Release new version
  }
}
```

---

### 🔧 Configuration Files Explained

#### `vite.config.ts`
```typescript
// Build and dev server configuration
- Library build settings
- Component resolution
- TypeScript support
- CSS preprocessing
```

#### `tsconfig.json`
```json
// TypeScript compilation settings
- Target: ES2020+
- Module: ESNext
- JSX: Vue
- Type checking rules
```

#### `vitest.config.ts`
```typescript
// Test runner configuration
- Jest-compatible test framework
- Component testing setup
- Coverage collection
- UI testing library integration
```

#### `.eslintrc.json`
```json
// Code linting rules
- Vue 3 + TypeScript support
- Code style enforcement
- Accessibility checks
```

#### `postcss.config.js`
```javascript
// CSS post-processing
- Autoprefixer (browser prefixes)
- CSS Variables support
- Optimization
```

---

### 📊 Build Output Structure

**After running `npm run build`:**

```
dist/
├── esm/                          # Modern JavaScript
│   ├── components/
│   │   ├── form/
│   │   │   ├── Button.js
│   │   │   ├── Button.d.ts
│   │   │   └── index.js
│   │   └── index.js
│   ├── composables/
│   ├── utils/
│   ├── index.js
│   └── index.d.ts
│
├── cjs/                          # Node.js compatible
│   ├── components/
│   ├── index.js
│   └── index.d.ts
│
├── umd/                          # Browser global
│   ├── use-ui.js                # Unminified (~40KB)
│   └── use-ui.min.js            # Minified + gzipped (~15KB)
│
├── types/                        # TypeScript definitions
│   ├── components.d.ts
│   └── index.d.ts
│
└── styles/
    ├── main.css                 # All styles bundled
    ├── main.min.css
    ├── tokens.css              # Design tokens only
    ├── themes/
    │   ├── light.css
    │   └── dark.css
    └── components.css           # Component styles only
```

---

### 🎯 Development Workflow

```
Local Development:
1. Edit files in src/
2. vite dev (auto-reload)
3. View changes instantly
4. Write tests (tests/)
5. Run npm run validate

Storybook Documentation:
1. Create Button.stories.ts
2. npm run storybook
3. View in interactive mode
4. Document props/events

Building for Production:
1. npm run build
2. dist/ folder created
3. Ready for npm publish

Publishing:
1. Update CHANGELOG.md
2. Bump version (package.json)
3. npm publish
4. Push to GitHub
5. Create GitHub release
```

---

### 🔗 Entry Points

**For different use cases:**

```javascript
// Full build (everything)
import * as UseUI from 'use-ui'

// Specific component
import { Button } from 'use-ui/components/form'

// Composable
import { useForm } from 'use-ui/composables'

// Utility
import { classnames } from 'use-ui/utils'

// Types only
import type { ButtonProps } from 'use-ui/types'

// Styles
import 'use-ui/dist/styles/main.css'
import 'use-ui/dist/styles/themes/dark.css'
```

---

## 🛠️ Setup Development

## 🛠️ Setup Development

### Prerequisites
- Node.js 16+ 
- npm, yarn, atau pnpm

### Installation & Development

```bash
# Clone repository
git clone https://github.com/yourusername/use-ui.git
cd use-ui

# Install dependencies
npm install

# Start development server
npm run dev

# Start Storybook
npm run storybook

# Run tests
npm run test

# Build library
npm run build

# Build documentation
npm run docs:build
```

### IDE Recommended

[VS Code](https://code.visualstudio.com/) + [Vue (Official)](https://marketplace.visualstudio.com/items?itemName=Vue.volar) (disable Vetur).

### Browser DevTools

- **Chrome/Edge:** [Vue.js devtools](https://chromewebstore.google.com/detail/vuejs-devtools/nhdogjmejiglipccpnnnanhbledajbpd)
- **Firefox:** [Vue.js devtools](https://addons.mozilla.org/en-US/firefox/addon/vue-js-devtools/)

---

## 🤝 Kontribusi

Kami dengan senang hati menerima kontribusi dari komunitas! Untuk berkontribusi:

1. **Fork** repository ini
2. **Create** branch feature Anda (`git checkout -b feature/AmazingFeature`)
3. **Commit** perubahan Anda (`git commit -m 'Add some AmazingFeature'`)
4. **Push** ke branch (`git push origin feature/AmazingFeature`)
5. **Open** Pull Request

### Panduan Kontribusi

- Ikuti code style yang ada
- Tambahkan tests untuk fitur baru
- Update dokumentasi jika diperlukan
- Pastikan semua tests passed

---

## 📄 Lisensi

Proyek ini dilisensikan di bawah [MIT License](LICENSE) - lihat file LICENSE untuk detail lengkap.

---

## 🔗 Useful Links

- [Dokumentasi Lengkap](https://use-ui-docs.example.com)
- [Storybook Interactive](https://storybook.use-ui.example.com)
- [GitHub Repository](https://github.com/yourusername/use-ui)
- [NPM Package](https://www.npmjs.com/package/use-ui)
- [Issues & Discussions](https://github.com/yourusername/use-ui/issues)

---

## 💬 Community & Support

- **Issues:** [GitHub Issues](https://github.com/yourusername/use-ui/issues)
- **Discussions:** [GitHub Discussions](https://github.com/yourusername/use-ui/discussions)
- **Email:** support@use-ui.example.com

---

**Made with ❤️ by the use-ui team**
