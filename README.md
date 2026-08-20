# WhatsApp-Exported-Chat-Converter-To-HTML-PDF

A Python script that seamlessly converts your exported WhatsApp chat logs (`.txt` files) and associated media into a beautiful, interactive, and easy-to-read HTML document that closely resembles the original WhatsApp UI. It also includes built-in functionality to easily download the chat as a highly optimized, clean PDF file or as an organized Excel log.

## Features

- **Cross-Platform Support**: Automatically detects and parses both iOS (`_chat.txt`) and Android (`<folder_name>.txt`) exported chat formats.
- **Media Integration**: Automatically embeds attached images, videos, audio (voice notes), and links to PDF files directly within the HTML chat bubbles.
- **WhatsApp UI Design**: Mimics the classic WhatsApp interface with distinct right/left aligned bubbles, colored sender names, and timestamp formatting.
- **One-Click PDF Export**: Includes a "Download PDF" button directly within the generated HTML file. When clicked, it opens the browser's print dialog.
- **Smart Excel Logging**: Automatically parses the conversation and creates an organized Excel (`.xlsx`) log where each message is categorized as an "Issue" or "Resolution" based on the sender.
- **Clickable Excel Images**: In the generated Excel log, images are seamlessly linked using absolute paths so you can open them with a single click right from the spreadsheet without messing up the Excel cell layout.
- **Embedded Downloads**: The Excel file is smartly embedded into the HTML file as a Data URI. This keeps your working directory clean from automatically generated Excel files until you explicitly click the "Download Excel" button!
- **Print-Optimized**: Contains specialized CSS (`@media print`) ensuring that chat bubbles and images are not awkwardly cut in half across pages, and removes the download buttons from the final PDF output.

## How to Use

1. **Export Your Chat**: Export your chat from WhatsApp on your phone, making sure to select **"Include Media"**.
2. **Extract Files**: Extract the `.zip` file into a new folder. Ensure the `.txt` file inside the folder is named exactly the same as the folder itself (e.g., if the folder is named `Chat`, the file must be `Chat.txt`) or `_chat.txt`.
3. **Install Requirements**: Install the necessary python packages:
   ```bash
   pip install -r requirements.txt
   ```
4. **Run the Script**: Place this folder in the same directory as the script and run:
   ```bash
   python whatsappChatToHTML.py
   ```
5. **Follow Prompts**: 
   - Select the folder containing your chat.
   - Select your name from the participant list to align your messages to the right.
6. **View & Save**: An HTML file (e.g., `Chat_v0.html`) will be generated. Open it in any modern web browser (like Chrome or Edge) to view your chat. 
   - Click **"📥 Download PDF"** at the top to save it as a PDF.
   - Click **"📊 Download Excel"** to instantly download the `.xlsx` log of the chat!

## Requirements

- Python 3.x
- `openpyxl`
- `pillow`

## Disclaimer
This script is intended for personal use. Please respect the privacy of the participants in the chat logs you choose to convert and save.
