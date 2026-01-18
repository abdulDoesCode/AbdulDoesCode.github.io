# Portfolio Website

A modern, responsive portfolio website designed to showcase both UX/UI design and frontend development projects. This is a multi-page website with an elegant layout that divides work into two main categories.

## Table of Contents
- [Features](#features)
- [Project Structure](#project-structure)
- [Pages Overview](#pages-overview)
- [Navigation Flow](#navigation-flow)
- [Technologies Used](#technologies-used)
- [Getting Started](#getting-started)
- [File Descriptions](#file-descriptions)
- [Customization](#customization)

## Features

✨ **Key Features:**
- **Responsive Design** - Works seamlessly on desktop, tablet, and mobile devices
- **Category-Based Organization** - Portfolio divided into two clear sections: UX/UI Design and Frontend Development
- **Project Grid Display** - Visual grid layout showcasing 6 projects per category
- **Dynamic Project Details** - Individual project pages with comprehensive information
- **Smooth Animations** - Modern hover effects and fade-in animations
- **Navigation System** - Easy-to-use navigation with active link highlighting
- **Modern Styling** - Gradient color scheme with professional purple and blue tones
- **Accessibility** - Semantic HTML5 and keyboard-friendly navigation

## Project Structure

```
New folder/
├── index.html              # Main landing page
├── ux-ui.html             # UX/UI Design projects showcase
├── frontend.html          # Frontend Development projects showcase
├── project-detail.html    # Dynamic project detail page
├── style.css              # Complete styling and responsive layout
├── script.js              # JavaScript functionality and interactions
└── README.md              # This file
```

## Pages Overview

### 1. **index.html** - Home Page
The main landing page featuring:
- **Navigation Header** - Logo and navigation links
- **Hero Section** - Welcome message and tagline
- **Introduction Section** - Brief overview of the portfolio
- **Portfolio Categories** - Two main cards linking to project categories:
  - UX/UI Design Projects
  - Frontend Development Projects
- **Contact Section** - Call-to-action with contact links
- **Footer** - Copyright information

### 2. **ux-ui.html** - UX/UI Design Projects
Showcases 6 UX/UI design projects in a responsive grid:
1. Mobile App Design
2. Dashboard Design
3. E-Commerce Platform
4. Fitness App UI
5. Social Media Redesign
6. Analytics Dashboard

Each project card includes:
- Custom SVG icon
- Project title
- Brief description
- Link to detailed project page

### 3. **frontend.html** - Frontend Development Projects
Showcases 6 frontend development projects in a responsive grid:
1. Interactive Game
2. Weather App
3. Portfolio Site
4. Todo List App
5. E-Commerce Store
6. Chart & Analytics

Each project card features similar layout to UX/UI page for consistency.

### 4. **project-detail.html** - Project Details Page
Dynamic page that displays comprehensive information for each project:
- **Back Navigation** - Easy way to return to project list
- **Project Title** - Name of the selected project
- **Detailed Content** - Includes:
  - Project overview
  - Objectives and goals
  - Design/development approach
  - Key features list
  - Results and impact metrics

Project details are loaded dynamically based on URL parameters (`?id=project-id`).

## Navigation Flow

```
Home (index.html)
├── Category Card 1: UX/UI Design
│   └── ux-ui.html (Project Grid)
│       └── Project Card → project-detail.html?id=uxui-1
│       └── Project Card → project-detail.html?id=uxui-2
│       └── ... (up to uxui-6)
│
├── Category Card 2: Frontend Development
│   └── frontend.html (Project Grid)
│       └── Project Card → project-detail.html?id=fe-1
│       └── Project Card → project-detail.html?id=fe-2
│       └── ... (up to fe-6)
│
└── Contact Section
    └── Email/Social Links
```

## Technologies Used

### Frontend Technologies:
- **HTML5** - Semantic markup
- **CSS3** - Styling with:
  - Flexbox for layouts
  - CSS Grid for project grids
  - Linear gradients
  - Smooth transitions
  - Media queries for responsiveness
- **JavaScript (ES6+)** - Interactivity including:
  - Smooth scrolling
  - DOM manipulation
  - URL parameter parsing
  - Intersection Observer API

### Icons:
- Custom SVG icons for visual appeal
- Scalable and lightweight

## Getting Started

### Prerequisites
- Modern web browser (Chrome, Firefox, Safari, Edge)
- No server or build tools required

### Setup Instructions

1. **Download/Extract Files**
   - Save all files in the same directory

2. **Open in Browser**
   - Open `index.html` in your web browser
   - Or double-click the `index.html` file

3. **Local Server (Optional)**
   - For best experience, run a local server:
   ```bash
   # Using Python 3
   python -m http.server 8000
   
   # Using Node.js (if installed)
   npx http-server
   ```
   - Then navigate to `http://localhost:8000`

## File Descriptions

### **index.html** (Main Landing Page)
- Entry point of the website
- Contains hero section and category introduction
- Links to both project showcase pages

### **ux-ui.html** (UX/UI Projects)
- Grid layout displaying 6 UX/UI design projects
- Each project card links to detailed project page
- Maintains consistent navigation across all pages

### **frontend.html** (Frontend Projects)
- Grid layout displaying 6 frontend development projects
- Same structure as UX/UI page for visual consistency
- All project cards link to detail pages

### **project-detail.html** (Project Information)
- Dynamic page using JavaScript to display content
- Reads project ID from URL parameters
- Contains comprehensive project information database
- Smooth back navigation

### **style.css** (Styling)
- **Color Scheme:**
  - Primary: `#667eea` (Purple)
  - Secondary: `#764ba2` (Violet)
  - Background: `#f7fafc` (Light Gray)
  - Text: `#2d3748` (Dark Gray)
  
- **Responsive Breakpoints:**
  - Mobile: < 768px
  - Tablet/Desktop: > 768px

- **Key CSS Classes:**
  - `.navbar` - Navigation bar
  - `.hero` - Hero section
  - `.category-card` - Category cards on home
  - `.project-item` - Individual project cards
  - `.project-detail` - Project detail page
  - `.footer` - Footer styling

### **script.js** (Interactivity)
- **Smooth Scrolling** - Smooth navigation to sections
- **Active Link Highlighting** - Shows current page
- **Hover Animations** - Interactive card effects
- **Fade-in Effects** - Scroll-triggered animations
- **Project Data Handling** - Manages all project information

## Customization

### Adding New Projects

1. **Add to UX/UI Projects:**
   - Edit `ux-ui.html`
   - Add new project card with unique ID
   - Add project data to `projectsData` in `project-detail.html`

2. **Add to Frontend Projects:**
   - Edit `frontend.html`
   - Follow same process as UX/UI

3. **Project Data Structure:**
   ```javascript
   'project-id': {
       title: 'Project Title',
       category: 'Category Name',
       description: `<h2>Overview</h2><p>Content...</p>`
   }
   ```

### Changing Colors

Edit the CSS variables in `style.css`:
```css
:root {
    --primary-color: #667eea;
    --secondary-color: #764ba2;
    --text-dark: #2d3748;
    --text-light: #718096;
    --bg-light: #f7fafc;
    --bg-white: #ffffff;
    --border-color: #e2e8f0;
    --hover-color: #5568d3;
}
```

### Modifying Contact Information

Update the contact links in `index.html`:
```html
<a href="mailto:your-email@example.com" class="contact-btn">Email Me</a>
<a href="your-linkedin-url" class="contact-btn">LinkedIn</a>
<a href="your-github-url" class="contact-btn">GitHub</a>
```

### Changing Font

Modify the font-family in `style.css`:
```css
body {
    font-family: 'Your Font Name', fallback-font, sans-serif;
}
```

## Browser Support

- ✅ Chrome (Latest)
- ✅ Firefox (Latest)
- ✅ Safari (Latest)
- ✅ Edge (Latest)
- ✅ Mobile Browsers

## Performance

- **Lightweight** - No external dependencies required
- **Fast Loading** - Minimal CSS and JavaScript
- **Optimized** - Efficient DOM manipulation
- **Responsive** - Mobile-first approach

## Tips for Best Results

1. **View on Different Devices** - Test on phone, tablet, and desktop
2. **Customize Projects** - Replace with your actual portfolio items
3. **Update Contact Info** - Add your real email and social links
4. **Test Navigation** - Verify all links work correctly
5. **Use Local Server** - For production deployment

## Future Enhancement Ideas

- Add project filtering/search functionality
- Implement image galleries for projects
- Add testimonials/client feedback section
- Create blog page for articles
- Add dark mode toggle
- Integrate with CMS for easier content management
- Add contact form with email integration
- Social media feeds integration

## License

This project is free to use and modify for personal and commercial purposes.

## Questions or Support

For questions about this portfolio website, refer to the HTML comments in each file or review the code structure for implementation details.

---

**Created:** January 2026
**Last Updated:** January 15, 2026
