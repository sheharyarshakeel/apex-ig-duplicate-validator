# APEX Interactive Grid Duplicate Detector 🚀

The seamless way to prevent duplicate entries in Oracle APEX Interactive Grids.

This plugin provides real-time, client-side validation for Interactive Grids (IG). It ensures data integrity by preventing users from entering duplicate values—whether based on a single column or a composite key of up to 5 columns—before the data even reaches the database.


[Demo](https://oracleapex.com/ords/r/sheharyar/learning/interactive-grid-plugin)

## Single Column Validation
![alt text](<https://github.com/oracle-apex-developer/apex-ig-duplicate-validator/blob/main/Single%20Column%20Validation.png>)

## Composite Column Validation
![alt text](<https://github.com/oracle-apex-developer/apex-ig-duplicate-validator/blob/main/Composite%20Column%20Validation.png>)


---

## ✨ Features

* ✅ **Real-time Validation** – Detects duplicates instantly as soon as a cell change occurs.
* ✅ **Composite Key Support** – Configure 1 to 5 columns to define what constitutes a "duplicate" (e.g., Project + Task + Date).
* ✅ **Visual Feedback** – Duplicate rows are automatically highlighted in red with a distinct left border for high visibility.
* ✅ **Native Save Blocking** – Uses the APEX native API to automatically block IG Save actions and Page Submissions.
* ✅ **Multi-IG Support** – Works independently on multiple Interactive Grids on the same page.
* ✅ **Universal Column Support** – Compatible with Text, Number, Select List, and Date columns.
* ✅ **Smart Comparison** – Case-insensitive matching and automatic whitespace handling (leading/trailing spaces ignored).
* ✅ **Customizable** – Configure your own custom error messages per IG instance.
* ✅ **Zero Dependencies** – Lightweight and fast; uses only built-in APEX JavaScript APIs.

---

## 🖥️ Compatibility

* **APEX Versions:** 24.1, 24.2+
* **Browsers:** All modern browsers (Chrome, Firefox, Edge, Safari)

---

## 📦 Installation

1. **Download** the plugin SQL file from the latest release.
2. Navigate to **Shared Components** > **Plug-ins**.
3. Click **Import** and upload the file.
4. Follow the wizard to install it into your application.

---

## ⚙️ How to Use

### 1. Set Region Static ID
* Navigate to your Interactive Grid region.
* In the Property Editor, go to **Attributes** > **Static ID**.
* Enter a unique ID (e.g., `MY_IG_REGION`).
    ## Single Column Validation
    ![alt text](<https://github.com/oracle-apex-developer/apex-ig-duplicate-validator/blob/main/Plugin_Setup_Image.png>)

### 2. Create Dynamic Action
* **Event:** `Change`
* **Selection Type:** `Region`
* **Region:** Select your Interactive Grid region.

### 3. Configure True Action
* **Action:** `IG Duplicate Detector [Plug-in]`
* **Columns 1–5:** Assign the columns that form your unique key.
* **Error Message:** Enter the text to display when a duplicate is found.

---

## 🤝 Contributing

Found a bug or have a feature request? Please open an issue or submit a pull request!

**Built for the APEX Community.**
