<p align="center">
  <img src="https://i.postimg.cc/XNZNV3TW/pic-i.jpg" width="380" alt="PIC INSPECTOR Logo">
</p>

<h1 align="center">PIC INSPECTOR</h1>
<p align="center">
  Advanced Image Metadata & OCR Analyzer (Forensics / Security Tool) 
  <br><br>
  Built with ❤️ by <b>BLACK ZER0 And HUNTER JACK</b>
</p>


---

## 📸 Overview
**PIC INSPECTOR** is a powerful Python-based image inspection tool that extracts, analyzes, and visualizes detailed metadata (EXIF) information from images.  
It also detects **suspicious data**, performs **OCR (text extraction)**, and pinpoints **GPS coordinates** embedded in photos — all with a beautiful **Rich TUI interface**.

---

## ⚙️ Features

✅ **EXIF Metadata Extraction** (via `exiftool`)  
✅ **Suspicious Metadata Detection** (malware or hidden payload patterns)  
✅ **GPS Coordinate Detection** with direct Google Maps link  
✅ **OCR Text Extraction** (via `pytesseract`)  
✅ **JSON / TXT Export** of metadata reports  
✅ **Beautiful CLI Interface** using `Rich` + `PyFiglet`  
✅ Works on **Termux**, **Linux**, and **Windows**


---

## 🔧 Installation

### 1️⃣ Install Required Packages
```bash
# For Termux / Linux:
pkg install python exiftool tesseract -y

# For Windows (PowerShell as Admin):
choco install exiftool tesseract -y
````

### 2️⃣ Clone or Download the Script

```bash
pkg install python exiftool tesseract -y
git clone https://github.com/<your-username>/Pic-INSPECTOR.git
cd Pic-INSPECTOR
chmod +x *
pip3 install -r requirements.txt
python3 pic-i.py
```

### 3️⃣ Install Python Dependencies

```bash
pip install rich pyfiglet pillow pytesseract
```

---

## ▶️ Usage

```bash
python pic-i.py
```

Then follow on-screen instructions:

```
[🧭] Enter image file path: example.jpg
```

📍 The tool will:

1. Extract all EXIF metadata
2. Detect suspicious entries
3. Perform OCR text extraction
4. Locate GPS info (if present)
5. Offer to save reports in JSON or TXT

---

## ⚠️ Suspicious Metadata Detection

The tool scans common metadata fields such as:

* `Comment`, `ImageDescription`, `Software`, `UserComment`, etc.
  And looks for **malicious keywords** like:

```
virus, malware, hidden, payload, backdoor, shell, hack, exploit, botnet, etc.
```

If any match is found → it’s flagged as:

```
[!! SUSPICIOUS]
```

---

## 🌍 GPS Example Output

```
✅ GPS location found
Latitude: 23° 45' 10.33" N
Longitude: 90° 23' 45.12" E
🌐 Open in Google Maps
```

---

## 🧩 File Saving

After analysis, you can export data:

* `info.json` → structured metadata
* `full_meta.txt` → full EXIF text dump

---

## 💻 Compatibility

| Platform                | Supported | Notes                             |
| ----------------------- | --------- | --------------------------------- |
| **Termux (Android)**    | ✅         | Best performance                  |
| **Linux (Ubuntu/Kali)** | ✅         | Recommended                       |
| **Windows 10+**         | ✅         | Use PowerShell                    |
| **macOS**               | ⚠️        | Requires manual setup of exiftool |

---

## 🧠 Example Output Preview

```
----------------------------------------
Full EXIF Metadata for example.jpg
----------------------------------------
[Software] Adobe Photoshop CC
[Comment] hidden payload detected [!! SUSPICIOUS]
[Make] Canon
[Model] EOS 80D
----------------------------------------
OCR Text Detected Inside Image:
"TOP SECRET FILE — DO NOT SHARE"
----------------------------------------
```
---
## 🖼️ DEMO PIC
<p align="center">
  <img src="https://i.postimg.cc/DyjtmbsD/Screenshot-2025-10-14-00-31-53-962-com-termux.jpg" alt="pic" width="45%" />
  &nbsp;&nbsp;
  <img src="https://i.postimg.cc/hvC3JHJz/Screenshot-2025-10-14-00-31-57-286-com-termux.jpg" alt="pic1" width="45%" />
</p>

---

## 🛡️ Credits

👨‍💻 **Code:** BLACK ZERO
🎯 **System:** HUNTER JACK
🧠 **Version:** 1.1
📅 **Release Date:** October 2025

---

## ⚠️ Disclaimer

This tool is created **for educational and forensic purposes only**.
The developers are **not responsible for misuse or illegal activity** involving this software.

---

## 🧾 License

This project is licensed under the **MIT License** — free to use, modify, and share with proper credit.

---

### ⭐ Support

If you find this tool useful, give it a star on GitHub 🌟
and follow for more cybersecurity tools by **BLACK ZERO** 🐉
