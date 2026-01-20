# QR_Generator_Webdev

# QR Code Generator (Node.js CLI)

This project is a simple **Node.js command-line app** that takes a URL from the user and generates:
- a QR code image file: `qr_img.png`
- a text file containing the entered URL: `URL.txt`

The user input is collected using `inquirer`, the QR code is generated using `qr-image`, and the files are saved using Node’s native `fs` module. :contentReference[oaicite:0]{index=0}

---

## What this project is

A CLI tool that:
1. Prompts the user to type a URL
2. Converts that URL into a QR code image
3. Saves both the QR image and the URL into files :contentReference[oaicite:1]{index=1}

---

## What you will see

- A terminal prompt: **"Type in your URL:"** :contentReference[oaicite:2]{index=2}  
- After entering a URL:
  - `qr_img.png` is created (QR code for your URL) :contentReference[oaicite:3]{index=3}  
  - `URL.txt` is created (stores the same URL you entered) :contentReference[oaicite:4]{index=4}  
  - Terminal message: **"The file has been saved!"** :contentReference[oaicite:5]{index=5}  

---

## How it works (based on your code)

- `inquirer.prompt()` asks for the URL input :contentReference[oaicite:6]{index=6}  
- `qr.image(url)` creates a QR image stream :contentReference[oaicite:7]{index=7}  
- `qr_svg.pipe(fs.createWriteStream("qr_img.png"))` writes the QR image to a PNG file :contentReference[oaicite:8]{index=8}  
- `fs.writeFile("URL.txt", url, ...)` saves the entered URL into a text file :contentReference[oaicite:9]{index=9}  

---

## Tech Stack

- **Node.js (ES Modules)** (`"type": "module"`) :contentReference[oaicite:10]{index=10}  
- **inquirer** (CLI input) :contentReference[oaicite:11]{index=11}  
- **qr-image** (QR generation) :contentReference[oaicite:12]{index=12}  
- **fs** (file saving) :contentReference[oaicite:13]{index=13}  

---

## Project Structure

```text
2.4-qr-code-project/
  index.js
  solution.js
  package.json
  package-lock.json
  qr_img.png
  URL.txt
