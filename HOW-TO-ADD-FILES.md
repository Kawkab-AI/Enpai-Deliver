# 📘 How to Add New HTML Files to Dashboard

## ✨ Super Easy 3-Step Process!

Your dashboard is now **dynamic** and works with **ANY file names** - not just user1.html, user2.html, etc.!

---

## 🎯 Step-by-Step Instructions

### Step 1: Add Your HTML File
Put your HTML file in the `html files/` folder.

**Examples of valid file names:**
- ✅ `john-report.html`
- ✅ `client-data-2024.html`
- ✅ `financial-summary.html`
- ✅ `project-alpha.html`
- ✅ `employee-records.html`
- ✅ ANY name you want!

### Step 2: Open `dashboard.html`
Find the configuration section around **line 188**. Look for this:

```javascript
const htmlFiles = [
    { fileName: 'user1.html', title: 'User Profile 1', subtitle: 'John Anderson', color: 'blue' },
    { fileName: 'user2.html', title: 'User Profile 2', subtitle: 'Sarah Mitchell', color: 'purple' },
    // ... more entries ...
];
```

### Step 3: Add Your Entry
Add a new line to the array:

```javascript
const htmlFiles = [
    { fileName: 'user1.html', title: 'User Profile 1', subtitle: 'John Anderson', color: 'blue' },
    { fileName: 'user2.html', title: 'User Profile 2', subtitle: 'Sarah Mitchell', color: 'purple' },
    // ... existing entries ...
    
    // YOUR NEW FILE:
    { fileName: 'my-file.html', title: 'My Title', subtitle: 'My Description', color: 'purple' }
];
```

**That's it! Done!** 🎉

---

## 🎨 Configuration Options

Each entry has 4 properties:

| Property | Description | Example |
|----------|-------------|---------|
| `fileName` | The name of your HTML file (inside "html files/" folder) | `'report.html'` |
| `title` | Main title shown on the card | `'Sales Report'` |
| `subtitle` | Subtitle/description shown on the card | `'Q4 2024'` |
| `color` | Color theme for the card | `'blue'` |

---

## 🌈 Available Colors

Choose from these colors:
- `'blue'` - Blue gradient
- `'purple'` - Purple gradient
- `'green'` - Green gradient
- `'pink'` - Pink gradient
- `'yellow'` - Yellow gradient
- `'indigo'` - Indigo gradient
- `'red'` - Red gradient
- `'teal'` - Teal gradient
- `'orange'` - Orange gradient
- `'cyan'` - Cyan gradient

---

## 📋 Complete Example

Let's say you have 3 new HTML files to add:
1. `sales-q4.html`
2. `team-overview.html`
3. `2024-summary.html`

**Here's what you add to the configuration:**

```javascript
const htmlFiles = [
    // Existing files
    { fileName: 'user1.html', title: 'User Profile 1', subtitle: 'John Anderson', color: 'blue' },
    { fileName: 'user2.html', title: 'User Profile 2', subtitle: 'Sarah Mitchell', color: 'purple' },
    // ... rest of existing files ...
    
    // NEW FILES - just add these 3 lines:
    { fileName: 'sales-q4.html', title: 'Sales Report Q4', subtitle: 'October-December 2024', color: 'green' },
    { fileName: 'team-overview.html', title: 'Team Overview', subtitle: 'Current Team Structure', color: 'orange' },
    { fileName: '2024-summary.html', title: 'Annual Summary', subtitle: 'Year 2024 Review', color: 'red' }
];
```

**Save the file and refresh your browser - the 3 new cards will appear automatically!** ✨

---

## 🔄 To Remove a File

Simply delete the line from the configuration or comment it out:

```javascript
const htmlFiles = [
    { fileName: 'user1.html', title: 'User Profile 1', subtitle: 'John Anderson', color: 'blue' },
    // { fileName: 'user2.html', title: 'User Profile 2', subtitle: 'Sarah Mitchell', color: 'purple' }, // COMMENTED OUT
    { fileName: 'user3.html', title: 'User Profile 3', subtitle: 'Michael Chen', color: 'green' },
];
```

---

## 💡 Pro Tips

1. **Keep your HTML files organized** in the `html files/` folder
2. **Use descriptive file names** so you remember what they are
3. **Match colors to content** (e.g., red for urgent, green for reports, blue for profiles)
4. **Test after adding** - just refresh the dashboard to see your changes
5. **No limit on files** - add as many as you need!

---

## ❓ FAQ

**Q: Can I use spaces in file names?**  
A: Yes, but use dashes instead (e.g., `my-file.html` not `my file.html`)

**Q: Do I need to restart anything?**  
A: No! Just refresh your browser after editing `dashboard.html`

**Q: What if I make a typo in the file name?**  
A: The button will show, but clicking it will show a "file not found" error. Just fix the typo in the configuration.

**Q: Can I change the order of cards?**  
A: Yes! Just rearrange the order of entries in the array.

**Q: Can I have duplicate titles?**  
A: Yes, but it's better to make them unique for clarity.

---

## 🎉 You're All Set!

Now you can easily manage unlimited HTML files on your dashboard without worrying about file naming conventions!

**Happy organizing!** 🚀

