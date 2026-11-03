<div align="center">
  <h1>💬 WhatsApp Chat Exporter to HTML, PDF & Excel</h1>
  <p>A powerful Python script that seamlessly converts your exported WhatsApp chat logs and associated media into a beautiful, interactive, and easy-to-read HTML document. It also features one-click PDF generation and smart Excel logging for professional record-keeping.</p>
</div>

---

## 🌟 Key Features

### 📱 Authentic WhatsApp UI
- **Right/Left Alignment:** Mimics the classic WhatsApp interface with distinct right/left aligned bubbles.
- **Visual Accuracy:** Retains colored sender names, timestamps, and overall chat flow.

### 📎 Seamless Media Integration
- **Images, Videos, & Audio:** Automatically embeds attached media directly within the HTML chat bubbles.
- **PDF Links:** Preserves links to attached PDF documents.

### 📊 Smart Excel Logging
- **Issue & Resolution Tracking:** Automatically parses the conversation and creates an organized Excel (`.xlsx`) log. Messages are categorized into "Issue" (client) or "Resolution" (support/you) rows.
- **Clickable Excel Images:** Images are perfectly linked using absolute paths so you can view them with a single click right from the spreadsheet without messing up the Excel cell layout!
- **Zero-Clutter Downloads:** The Excel file is cleverly embedded into the HTML file as a Data URI. Your working directory stays clean until you explicitly click the "Download Excel" button!

### 📥 One-Click Exports
- **Download PDF:** Includes a button directly within the generated HTML file. When clicked, it opens the browser's print dialog.
- **Print-Optimized CSS:** Specialized `@media print` rules ensure that chat bubbles and images are not awkwardly cut in half across pages, and removes the download buttons from the final PDF output.
- **Download Excel:** Instantly extract the conversation log to an `.xlsx` file.

### 🌍 Cross-Platform Compatibility
- Automatically detects and parses both **iOS (`_chat.txt`)** and **Android (`<folder_name>.txt`)** exported chat formats.

---

## 🛠️ Tech Stack & Requirements

- **Core Language:** Python 3.x
- **Required Libraries:**
  - `openpyxl` (For generating structured Excel files)
  - `pillow` (For image processing)

---

## 📸 App Screenshots

*(Note: Replace these placeholders with actual screenshots of your generated HTML page, PDF output, and Excel file)*
<div align="center">
  <img src="https://via.placeholder.com/250x500?text=HTML+View" width="30%">
  <img src="https://via.placeholder.com/250x500?text=PDF+Export" width="30%">
  <img src="https://via.placeholder.com/250x500?text=Excel+Log" width="30%">
</div>

---

## 🚀 How to Run

1. **Export Your Chat**: Export your chat from WhatsApp on your phone. Make sure to select **"Include Media"**.
2. **Extract Files**: Extract the `.zip` file into a new folder. Ensure the `.txt` file inside the folder is named exactly the same as the folder itself (e.g., if the folder is named `Chat`, the file must be `Chat.txt`) or `_chat.txt`.
3. **Install Requirements**:
   Open your terminal and install the required packages:
   ```bash
   pip install -r requirements.txt
   ```
4. **Run the Script**: 
   Place your extracted chat folder in the same directory as the script and run:
   ```bash
   python whatsappChatToHTML.py
   ```
5. **Follow Prompts**: 
   - Select the folder containing your chat.
   - Select your name from the participant list to align your messages to the right side of the screen.
6. **View & Save**: 
   An HTML file (e.g., `Chat_v0.html`) will be generated. Open it in any modern web browser (like Chrome, Edge, or Safari) to view your chat. 

---

## ⚠️ Disclaimer
This script is intended for personal and professional record-keeping use. Please respect the privacy of the participants in the chat logs you choose to convert and save.

## 🤝 Contact / Support
Created for seamless chat logging and management. Feel free to fork, modify, and contribute to the repository!
