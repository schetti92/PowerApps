# Welcome to My Power Platform Sandbox 🚀

This is your go-to playground for exploring, experimenting, and building in the world of Microsoft Power Platform! Here, you’ll find a collection of sample projects, reusable components, and tools designed to inspire creativity, encourage learning, and speed up your development process. Whether you're here to tinker with Power Apps, automate tasks with Power Automate, visualize data with Power BI, or delve into custom development, this sandbox has you covered.

### What’s Inside
- **Sample Projects**: Fully functional projects that demonstrate Power Platform capabilities and help you kickstart your own ideas.
- **Reusable Components**: Ready-to-use components designed for efficiency and easy integration into your Power Platform solutions.
- **Hands-on Practice**: Experiment with and modify components to suit your needs or create something entirely new. This is your space to explore freely.

Feel free to experiment, break, rebuild, and learn. Make this repository your own personal Power Platform playground, where your skills grow, and ideas come to life!

### Sample Projects

- **[Top Navigation Menu Component](https://github.com/schetti92/PowerApps/tree/main/TopNavBarMenuPowerapps)**
- **[Expandable Left Navigation Component ](https://github.com/schetti92/PowerApps/tree/main/ExpandableLeftNavComponent)**
- **[PTE Like Essay writting App using PowerApps and Generative AI](https://github.com/schetti92/PowerApps/tree/main/EssayWritingApp)**
- **[Chat Application - With SharePoint Lists](https://github.com/schetti92/PowerApps/tree/main/ChatApplication)**
- **[Recipe Wizard using PowerApps and Generative AI](https://github.com/schetti92/PowerApps/tree/main/RecipeWizardApp)**


# 📌 PowerApps Responsive Design Cheat Sheet

A collection of **PowerApps formulas and techniques** to create fully **responsive** canvas apps. 🚀

---

## 📏 General Responsive Formulas
### 🔹 Center Objects
- **Center Horizontally:**  
  ```powerapps
  X = Parent.Width / 2 - Self.Width / 2
  ```
- **Center Vertically:**  
  ```powerapps
  Y = Parent.Height / 2 - Self.Height / 2
  ```

### 🔹 Relative Positioning
- **Position below another control:**  
  ```powerapps
  Y = Label1.Y + Label1.Height + 10
  ```
- **Position next to another control:**  
  ```powerapps
  X = Label1.X + Label1.Width + 10
  ```

### 🔹 Dynamic Width & Height
- **Make a control full width:**  
  ```powerapps
  Width = Parent.Width
  ```
- **Make a control half the screen width:**  
  ```powerapps
  Width = Parent.Width / 2
  ```
- **Set a control’s height dynamically:**  
  ```powerapps
  Height = Parent.Height * 0.2
  ```

### 🔹 Grid-Based Layout
- **Three equal columns:**  
  ```powerapps
  Width = Parent.Width / 3
  ```
- **Two columns (Left 70%, Right 30%):**  
  ```powerapps
  Left Column: Width = Parent.Width * 0.7
  Right Column: Width = Parent.Width * 0.3
  ```

---

## 📱 Device Adaptability
### 🔹 Detect Screen Size
- **Check if device is Phone or Tablet:**  
  ```powerapps
  If(App.Width < 600, "Phone", "Tablet")
  ```
- **Change layout based on width:**  
  ```powerapps
  If(App.Width > 1200, "Desktop", 
     App.Width > 600, "Tablet", 
     "Phone")
  ```

### 🔹 Adjust Font Size Based on Screen
- **Make text responsive:**  
  ```powerapps
  FontSize = Parent.Width * 0.05
  ```
- **Title font vs. normal text:**  
  ```powerapps
  Title: FontSize = Parent.Width * 0.08
  Body: FontSize = Parent.Width * 0.04
  ```

### 🔹 Adjust Button Size
- **Dynamic button width:**  
  ```powerapps
  Width = Parent.Width * 0.25
  ```
- **Dynamic button height:**  
  ```powerapps
  Height = Parent.Height * 0.1
  ```

---

## 📂 Containers & Flexible Layouts
### 🔹 Auto-Adjustable Gallery
- **Gallery with dynamic columns:**  
  ```powerapps
  WrapCount = If(App.Width > 1200, 4, If(App.Width > 800, 3, 2))
  ```

### 🔹 Hide/Show Components Based on Screen Size
- **Show extra menu on larger screens:**  
  ```powerapps
  Visible = If(App.Width > 900, true, false)
  ```
- **Switch between vertical and horizontal layout dynamically:**  
  ```powerapps
  Layout = If(App.Width > 900, Layout.Horizontal, Layout.Vertical)
  ```

---

## 🎨 Styling & Aesthetics
### 🔹 Responsive Border Radius
- **Make images & buttons rounded:**  
  ```powerapps
  BorderRadius = Min(Self.Width, Self.Height) / 2
  ```
- **Soft edges for all components:**  
  ```powerapps
  BorderRadius = Parent.Width * 0.02
  ```

### 🔹 Shadow & Elevation
- **Dynamic shadow effect:**  
  ```powerapps
  Fill = RGBA(0, 0, 0, 0.1 * (App.Width / 1200))
  ```

---

## 🎛 Advanced Responsive Techniques
### 🔹 Flexible Side Menu
- **Hide menu on mobile, show on desktop:**  
  ```powerapps
  Visible = App.Width > 800
  ```
- **Make sidebar 20% of screen width:**  
  ```powerapps
  Width = Parent.Width * 0.2
  ```

### 🔹 Dynamic Image Resizing
- **Make an image fill 50% of screen width while maintaining aspect ratio:**  
  ```powerapps
  Width = Parent.Width * 0.5
  Height = Width * (Image1.Height / Image1.Width)
  ```

---

## 🔹 Best Practices for Responsiveness
✅ **Use `Parent.Width` & `Parent.Height` instead of fixed values**  
✅ **Use `If(App.Width < X, Small Layout, Large Layout)` for conditional changes**  
✅ **Leverage containers (flexible layouts) to structure content properly**  
✅ **Test on different screen sizes before publishing**  


## Regards - Shashika Hettiarachchi ❤️

