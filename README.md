# Engineer Blogger Template

A modern, dark-themed technical blog and portfolio template for [Blogger](https://blogger.com). Designed for engineers, CS students, and makers to document projects in embedded systems, electronics, IoT security, and computer science.

![Dark Theme](https://img.shields.io/badge/Theme-Dark-0d1117?style=flat-square)
![Blogger](https://img.shields.io/badge/Platform-Blogger-FF5722?style=flat-square&logo=blogger)
![License](https://img.shields.io/badge/License-MIT-green?style=flat-square)

---

## ✨ Features

- 🌑 **Modern dark theme** — GitHub-inspired color palette
- 📱 **Fully responsive** — hamburger menu, single-column mobile layout
- 🗂️ **Category filtering** — Electronics, Embedded Systems, CS, IoT & Security
- 📄 **Standalone About & Contact pages** — auto-detected, no HTML editing needed
- 💻 **Code blocks** — dark background, monospace font, one-click Copy button
- ⚡ **Fast** — vanilla CSS & JS, zero dependencies beyond Font Awesome & Google Fonts
- 🔖 **Sidebar** — author card, categories, popular posts, tag cloud

---

## 🚀 Quick Start

### 1. Configure your details
Open `EngineerBlog.xml` and find the `CONFIGURATION` block near the top. Fill in your details:

```xml
<!-- ╔══════════════════════════════════════╗
     ║        CONFIGURATION BLOCK           ║
     ╚══════════════════════════════════════╝
  AUTHOR_NAME        : Your full name
  AUTHOR_ROLE        : Your title/degree
  AUTHOR_SUBTITLE    : e.g. "Embedded Systems | PCB Design"
  AUTHOR_BIO         : Short bio for sidebar
  AUTHOR_UNIVERSITY  : Your institution
  AUTHOR_PHOTO_URL   : Direct URL to your profile picture
  PORTFOLIO_URL      : Your external portfolio/website
  GITHUB_URL         : https://github.com/yourusername
  LINKEDIN_URL       : https://www.linkedin.com/in/yourprofile/
  EMAIL              : your.email@example.com
  HERO_TITLE         : Heading shown on homepage
  HERO_TAGLINE       : Subtitle shown on homepage
  YEAR               : Copyright year
-->
```

### 2. Upload to Blogger
1. Go to **Blogger Dashboard → Theme → Edit HTML**
2. Select all existing code and delete it
3. Paste the entire contents of `EngineerBlog.xml`
4. Click **Save**

### 3. Create Static Pages
Go to **Pages → New Page** and create two pages with **exactly** these titles (case-sensitive):

| Title | Purpose |
|-------|---------|
| `About` | Renders the full About Me page automatically |
| `Contact` | Renders the full Contact page automatically |

> Leave the page body **empty** — the template injects the content for you.

### 4. Label your posts
Use these exact **Labels** when publishing posts to enable category filtering:

| Label | Category |
|-------|---------|
| `Electronics` | Circuit design, PCB, power electronics |
| `Embedded-Systems` | Arduino, ESP32, Raspberry Pi, microcontrollers |
| `Computer-Science` | Programming, algorithms, software |
| `IoT-Security` | IoT experiments, hardware security, ethical hacking |
| `Blog` | General posts |

---

## 🎨 Code Blocks in Posts

When editing a post in HTML mode, wrap code like this:

```html
<pre><code>
void setup() {
  Serial.begin(115200);
  pinMode(LED_BUILTIN, OUTPUT);
}
</code></pre>
```

The template automatically adds a **Copy** button to every `<pre><code>` block.

---

## 📁 File Structure

```
engineer-blogger-template/
├── EngineerBlog.xml   # Main Blogger template — upload this
├── README.md          # This file
├── .gitignore         # Hides OS/IDE junk files from git
└── LICENSE            # MIT License
```

---

## 🛠️ Customization Tips

| What to change | Where in the XML |
|----------------|-----------------|
| Accent color (purple) | `:root { --accent: #7c6af7; }` |
| Green accent | `:root { --green: #3fb950; }` |
| Background color | `:root { --bg: #0d1117; }` |
| Nav categories | `eb-nav-links` section |
| Footer description | `eb-footer-desc` section |

---

## 📋 Requirements

- A free [Blogger](https://blogger.com) account
- Google account to manage the blog
- No server, no build tools, no Node.js needed

---

## 📄 License

[MIT](LICENSE) — free to use, modify, and share. Credit appreciated but not required.
