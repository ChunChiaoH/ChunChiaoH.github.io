# Jekyll Site Structure & Flow Diagram

```
┌─────────────────────────────────────────────────────────────────┐
│                        JEKYLL BUILD PROCESS                     │
└─────────────────────────────────────────────────────────────────┘

1. CONFIGURATION & SETUP
   _config.yml ──────────► Controls entire site
   │                       │
   ├─ Theme: minimal-mistakes
   ├─ Author: Joe Huang  
   ├─ Plugins: feed, sitemap, etc.
   └─ Site settings

2. CONTENT STRUCTURE
   ┌─────────────────┐    ┌─────────────────┐    ┌─────────────────┐
   │   CONTENT       │    │    LAYOUTS      │    │   INCLUDES      │
   │                 │    │                 │    │                 │
   │ index.html ────────► │ home.html       │    │ header.html     │
   │ _posts/        │    │ single.html     │    │ footer.html     │
   │ _pages/        │    │ archive.html    │    │ sidebar.html    │
   │ _data/         │    │ default.html    │    │ navigation.html │
   └─────────────────┘    └─────────────────┘    └─────────────────┘
            │                       │                       │
            └───────────────────────┼───────────────────────┘
                                    ▼
   ┌─────────────────────────────────────────────────────────────────┐
   │                    JEKYLL PROCESSING                            │
   │  • Converts Markdown to HTML                                    │
   │  • Applies layouts to content                                   │
   │  • Processes Liquid templating                                  │
   │  • Compiles Sass to CSS                                         │
   └─────────────────────────────────────────────────────────────────┘
                                    │
                                    ▼
3. STYLING & ASSETS
   ┌─────────────────┐              ┌─────────────────┐
   │   SASS/CSS      │              │    ASSETS       │
   │                 │              │                 │
   │ _sass/          │──────────────┤ assets/css/     │
   │ minimal-mistakes│              │ assets/js/      │
   │ skins & styles  │              │ assets/images/  │
   └─────────────────┘              └─────────────────┘
                                    │
                                    ▼
   ┌─────────────────────────────────────────────────────────────────┐
   │                     FINAL WEBSITE                               │
   │  Static HTML files ready for hosting on GitHub Pages           │
   └─────────────────────────────────────────────────────────────────┘
```

## 🚀 WHERE TO START IMPROVING YOUR WEBSITE

### **IMMEDIATE WINS (Start Here!)**

1. **📝 Update Homepage Content**
   ```
   📁 index.html
   └── Add more engaging introduction
   └── Add call-to-action buttons
   └── Showcase your projects/skills
   ```

2. **👤 Complete Author Profile**
   ```
   📁 _config.yml (lines 115-140)
   └── Add professional avatar image
   └── Write compelling bio
   └── Link your GitHub, LinkedIn profiles
   └── Add your website URL
   ```

3. **📄 Create Essential Pages**
   ```
   📁 _pages/ (create these)
   ├── about.md ─────── Your background, experience
   ├── projects.md ──── Showcase your work
   ├── resume.md ────── Professional experience
   └── contact.md ───── How to reach you
   ```

### **CONTENT IMPROVEMENTS**

4. **📰 Add Blog Posts**
   ```
   📁 _posts/
   └── Write about your projects, learnings, tutorials
   └── Format: YYYY-MM-DD-title.md
   ```

5. **🎨 Customize Appearance**
   ```
   📁 _config.yml
   └── Change skin theme (line 15)
   └── Add site logo (line 29)
   └── Customize colors in _sass/
   ```

### **ADVANCED IMPROVEMENTS**

6. **🔧 Add Custom Features**
   ```
   📁 _includes/
   └── Custom navigation
   └── Project showcase components
   └── Skills section
   ```

7. **📊 Add Analytics & SEO**
   ```
   📁 _config.yml
   └── Google Analytics (lines 107-111)
   └── SEO verification (lines 84-89)
   └── Social media integration
   ```

## 🎯 RECOMMENDED ORDER OF IMPROVEMENT

```
1. Update _config.yml (author info, links)
     ↓
2. Improve index.html content
     ↓
3. Create about.md and projects.md pages
     ↓
4. Add professional avatar image
     ↓
5. Write your first blog post
     ↓
6. Customize theme and colors
     ↓
7. Add advanced features (analytics, custom sections)
```

## 🛠️ FILES TO FOCUS ON

| Priority | File | Purpose |
|----------|------|---------|
| 🔥 HIGH | `_config.yml` | Site settings, author info |
| 🔥 HIGH | `index.html` | Homepage content |
| 🔥 HIGH | `_pages/about.md` | About you page |
| 🔥 HIGH | `assets/images/` | Add your photos |
| 🟡 MEDIUM | `_posts/` | Blog content |
| 🟡 MEDIUM | `_data/navigation.yml` | Custom menu |
| 🟢 LOW | `_sass/` | Advanced styling |
| 🟢 LOW | `_includes/` | Custom components |

Start with the HIGH priority files and work your way down!