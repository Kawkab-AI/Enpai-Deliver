# Kawkab Dashboard - Professional Website

A stunning, modern, and fully responsive dashboard website with authentication.

## 🚀 Features

- **Elegant Login Page** with smooth animations
- **Protected Dashboard** with glassmorphism navbar
- **10 User Profile Pages** with beautiful card layouts
- **Responsive Design** for all devices
- **Modern UI/UX** with TailwindCSS
- **Client-side Authentication** (demo purposes)

## 📁 Project Structure

```
Deliver/
│
├── index.html              # Login page (entry point)
├── dashboard.html          # Main dashboard with dynamic card generation
├── README.md               # This file
│
└── html files/             # Folder containing all user profile pages
    ├── user1.html          # John Anderson - Senior Software Engineer
    ├── user2.html          # Sarah Mitchell - Product Manager
    ├── user3.html          # Michael Chen - Data Scientist
    ├── user4.html          # Emma Davis - UX/UI Designer
    ├── user5.html          # David Wilson - DevOps Engineer
    ├── user6.html          # Lisa Thompson - Marketing Director
    ├── user7.html          # James Rodriguez - Sales Manager
    ├── user8.html          # Sophia Martinez - HR Manager
    ├── user9.html          # Robert Taylor - Financial Analyst
    ├── user10.html         # Jessica Brown - Customer Success Manager
    └── (add your own HTML files here with any name)
```



## 🎨 Customization Guide

### 1. **Add New HTML Files (ANY NAME!) - Super Easy! 🚀**

**The dashboard now works with ANY file names - not just user1, user2, etc!**

To add a new HTML file to the dashboard:

1. **Upload your HTML file** to the `html files/` folder (you can name it anything: `john-report.html`, `client-data.html`, `2024-summary.html`, etc.)

2. **Open `dashboard.html`** and find the configuration section (around line 188)

3. **Add a new entry** to the `htmlFiles` array:

```javascript
const htmlFiles = [
    { fileName: 'user1.html', title: 'User Profile 1', subtitle: 'John Anderson', color: 'blue' },
    // ... existing entries ...
    // ADD YOUR NEW FILE HERE:
    { fileName: 'my-custom-file.html', title: 'My Custom Page', subtitle: 'Any Description', color: 'purple' }
];
```

**That's it!** The card will automatically appear on the dashboard with all styling and animations! 🎉

**Available Colors:** blue, purple, green, pink, yellow, indigo, red, teal, orange, cyan

### 2. **Change Logos in Navbar**

Open `dashboard.html` and locate these sections:

**Left Logo (Line ~62-73):**
```html
<div class="logo-placeholder flex items-center space-x-3">
    <!-- Replace this div with your logo image -->
    <img src="your-left-logo.png" alt="Logo" class="h-12">
</div>
```

**Right Logo (Line ~77-88):**
```html
<div class="logo-placeholder flex items-center space-x-3">
    <!-- Replace this div with your logo image -->
    <img src="your-right-logo.png" alt="Logo" class="h-12">
</div>
```

### 3. **Update User Profiles**

Each user file in the `html files/` folder contains:
- Name
- Title
- Email
- Phone
- Location
- Department
- About section

Simply edit the HTML content in each file to match your real user data.

Replace with your desired credentials.

### 5. **Modify Color Scheme**

The website uses gradient colors. To change them:
- **Login page background:** Edit the `body` gradient in `index.html`
- **Dashboard background:** Edit the `body` gradient in `dashboard.html`
- **Card colors:** Choose from available colors when adding files (see step 1)

## 🌐 How to Run

1. **Open the website:**
   - Simply open `index.html` in your web browser
   - Or use a local server for better experience

2. **Using Live Server (Recommended):**
   ```bash
   # If you have VS Code with Live Server extension
   # Right-click on index.html and select "Open with Live Server"
   ```

3. **Or use Python HTTP Server:**
   ```bash
   python -m http.server 8000
   # Then open http://localhost:8000
   ```

## 🎯 User Flow

1. User visits `index.html` (Login Page)
3. Gets redirected to `dashboard.html`
4. Sees 10 user cards with "View Profile" buttons
5. Clicks any card to open the user profile in a new tab
6. Can logout using the logout button

## 📱 Responsive Design

The website is fully responsive and works on:
- 📱 Mobile devices
- 📱 Tablets
- 💻 Desktops
- 🖥️ Large screens

## 🎨 Design Features

- **Glassmorphism** navbar effect
- **Smooth animations** on hover and page load
- **Gradient backgrounds** throughout
- **Card hover effects** with elevation
- **Professional typography** using Inter font
- **Modern color palette** with vibrant gradients

## 🔒 Security Note

⚠️ **Important:** This is a client-side authentication demo only. For production use, you must implement proper backend authentication with:
- Server-side validation
- Encrypted passwords
- Secure session management
- HTTPS

## 💡 Tips

- All HTML files use TailwindCSS via CDN (no build step required)
- Images and logos should be placed in the same directory
- Session storage is used to maintain login state
- Clear browser session storage to "logout" without the button

## 📞 Support

For customization help or questions, refer to:
- [TailwindCSS Documentation](https://tailwindcss.com/docs)
- [MDN Web Docs](https://developer.mozilla.org/)

---

**Built with ❤️ using TailwindCSS and modern web technologies**

© 2025 Kawkab.AI - All Rights Reserved

