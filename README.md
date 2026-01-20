# QR_Generator_Webdev

This is a simple **command-line QR Code Generator** built with **Node.js**. It asks the user to enter a URL in the terminal, then generates:
- a QR code image file (`qr_img.png`)
- a text file containing the same URL (`URL.txt`)

---

## What this project does

- Takes a URL input using a terminal prompt
- Generates a QR code for the URL
- Saves the URL in a text file for reference

---

## Tech Used

- **Node.js**
- **inquirer** (to take input from terminal)
- **qr-image** (to generate QR code)
- **fs** (to create and write files)

---

## Project Files

```text
qr-project/
  solution.js
  index.js
  package.json
  package-lock.json
  README.md

Generated after running:
- `URL.txt`
- `qr_img.png`
```

## Steps to Run (Windows PowerShell)

```powershell
# 1) Go to your project folder
cd "C:\Users\Grishma\OneDrive\Desktop\qr-project"

# 2) (Optional) Check files
ls

# 3) Install required packages
npm install inquirer qr-image

# 4) (Optional) If you installed express as well
npm i express

# 5) Run the program
node solution.js

# 6) Enter a URL when prompted
? Type in your URL: https://example.com

```

## Output

- `URL.txt`  
  Stores the URL you entered.

- `qr_img.png`  
  QR code image generated for the URL.

---

## Developer
Grishma C.D

