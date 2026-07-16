# 🎨 use-ui

**use-ui** adalah library komponen template UI modern yang dirancang untuk kemudahan penggunaan dan fleksibilitas tinggi. Proyek ini menggabungkan best practices dalam **Design System**, **Dokumentasi API**, dan **Implementasi lintas framework**.

> ✨ **Fokus:** HTML + CSS yang elegan | **Tujuan:** Mudah digunakan across platforms | **Status:** Aktif dikembangkan

---

## 📋 Daftar Isi

- [Project Overview](#project-overview)
- [Fitur Utama](#fitur-utama)
- [Instalasi](#instalasi)
- [Quick Start](#quick-start)
- [Design System](#design-system)
- [Struktur Komponen](#struktur-komponen)
- [Dokumentasi API](#dokumentasi-api)
- [Dukungan Lintas Framework](#dukungan-lintas-framework)
- [Struktur Proyek](#struktur-proyek)
- [Setup Development](#setup-development)
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

## ✨ Fitur Utama

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

### NPM
```bash
npm install use-ui
```

### Yarn
```bash
yarn add use-ui
```

### PNPM
```bash
pnpm add use-ui
```

---

## 🚀 Quick Start

### Vue 3 Setup

```javascript
// main.js
import { createApp } from 'vue'
import useUI from 'use-ui'
import 'use-ui/dist/style.css'
import App from './App.vue'

const app = createApp(App)

app.use(useUI)
app.mount('#app')
```

### Menggunakan Komponen

```vue
<template>
  <div class="container">
    <UseButton type="primary" @click="handleClick">
      Click Me!
    </UseButton>
    
    <UseCard title="Welcome">
      <p>Ini adalah contoh menggunakan use-ui components</p>
    </UseCard>
    
    <UseInput 
      v-model="username" 
      placeholder="Masukkan username"
      label="Username"
    />
  </div>
</template>

<script setup>
import { ref } from 'vue'

const username = ref('')

const handleClick = () => {
  console.log('Button clicked!')
}
</script>
```

---

## 🎨 Design System

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

### Kategori Komponen

#### Form Components
- `UseInput` - Text input field
- `UseSelect` - Dropdown selection
- `UseCheckbox` - Checkbox control
- `UseRadio` - Radio button
- `UseTextarea` - Multi-line text input
- `UseSwitch` - Toggle switch
- `UseForm` - Form wrapper dengan validation

#### Layout Components
- `UseContainer` - Container dengan max-width
- `UseGrid` - Grid layout system
- `UseStack` - Stack layout (vertical/horizontal)
- `UseCard` - Card component
- `UseSpacer` - Space component

#### Navigation Components
- `UseButton` - Button component
- `UseNavbar` - Top navigation bar
- `UseSidebar` - Side navigation
- `UseBreadcrumb` - Breadcrumb trail
- `UseMenu` - Dropdown menu

#### Feedback Components
- `UseToast` - Toast notification
- `UseAlert` - Alert message
- `UseModal` - Modal dialog
- `UsePopover` - Popover overlay
- `UseTooltip` - Tooltip information
- `UseProgress` - Progress bar
- `UseSkeleton` - Loading skeleton

#### Data Display
- `UseTable` - Data table component
- `UsePagination` - Pagination control
- `UseBadge` - Badge component
- `UseTag` - Tag component
- `UseAvatar` - Avatar component
- `UseList` - List component

---

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

### Instalasi Framework-Specific

#### Vue 3
```bash
npm install use-ui @use-ui/vue3
```

#### React
```bash
npm install use-ui @use-ui/react
```

#### Angular
```bash
npm install use-ui @use-ui/angular
```

#### Vanilla JS (Web Components)
```bash
npm install use-ui
```

### Contoh Implementasi

#### React
```jsx
import { UseButton, UseInput } from '@use-ui/react'
import '@use-ui/react/dist/style.css'

export function MyComponent() {
  const [name, setName] = useState('')

  return (
    <>
      <UseInput 
        value={name}
        onChange={(e) => setName(e.target.value)}
        placeholder="Enter your name"
      />
      <UseButton onClick={() => alert(name)}>
        Submit
      </UseButton>
    </>
  )
}
```

#### Angular
```typescript
import { Component } from '@angular/core'
import { UseUIModule } from '@use-ui/angular'

@Component({
  selector: 'app-root',
  template: `
    <use-button (click)="handleClick()">
      Click Me
    </use-button>
  `,
  standalone: true,
  imports: [UseUIModule]
})
export class AppComponent {
  handleClick() {
    console.log('Button clicked!')
  }
}
```

#### Vanilla JavaScript
```html
<script src="https://cdn.jsdelivr.net/npm/use-ui/dist/use-ui.js"></script>
<link rel="stylesheet" href="https://cdn.jsdelivr.net/npm/use-ui/dist/style.css">

<script>
  const button = document.createElement('use-button')
  button.textContent = 'Click Me'
  button.addEventListener('click', () => {
    console.log('Button clicked!')
  })
  document.body.appendChild(button)
</script>
```

---

## 📁 Struktur Proyek

```
use-ui/
├── src/
│   ├── components/           # Komponen UI
│   │   ├── Button/
│   │   ├── Input/
│   │   ├── Card/
│   │   ├── Modal/
│   │   ├── Toast/
│   │   └── ...
│   ├── styles/              # CSS & Design System
│   │   ├── variables.css    # CSS Variables
│   │   ├── base.css         # Base styles
│   │   ├── components.css   # Component styles
│   │   └── utilities.css    # Utility classes
│   ├── composables/         # Vue Composables
│   │   ├── useForm.js
│   │   ├── useModal.js
│   │   └── ...
│   ├── utils/              # Helper functions
│   │   ├── validation.js
│   │   ├── formatting.js
│   │   └── ...
│   ├── App.vue
│   └── main.js
├── docs/                    # Dokumentasi
│   ├── guide/
│   ├── api/
│   └── examples/
├── .storybook/              # Storybook configuration
├── tests/                   # Unit tests
├── package.json
├── vite.config.js
└── README.md
```

---

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
