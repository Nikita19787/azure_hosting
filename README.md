# 🌐 Static Website Hosting using Microsoft Azure Blob Storage

---

## 📌 Overview

This project demonstrates how to deploy a static website using Microsoft Azure's *Blob Storage* with the *Static Website Hosting* feature. It’s a beginner-friendly project that helps you understand Azure Storage services and deploy front-end code (HTML, CSS, JavaScript) without a web server.

---

## 🧰 Technologies & Tools Used

- *Microsoft Azure*
  - Storage Account
  - Blob Storage (Static Website Hosting)
- *HTML, CSS, JavaScript* (Basic Website Files)
- *Azure Portal*
- *VS Code* (or any code editor)

---

## 🎯 Objectives

- Create and configure an Azure Storage Account.
- Enable Static Website Hosting.
- Upload static files (HTML/CSS/JS) to the $web container.
- Access and verify website via the public URL.

---

## 🛠 Step-by-Step Implementation

### 1. *Create an Azure Storage Account*

- Go to [Azure Portal](https://portal.azure.com)
- Navigate to Storage accounts > + Create
- Fill in the details:
  - *Subscription*: Select your subscription
  - *Resource group*: Create new or use existing
  - *Storage account name*: Must be globally unique
  - *Region*: Choose nearest data center
  - *Performance*: Standard
  - *Redundancy*: LRS (Locally Redundant Storage)

Click *Review + Create, then **Create*.

---

### 2. *Enable Static Website Hosting*

- Go to your created *Storage Account*
- In the left panel, find *"Static website"*
- Click *Enable*
- Enter the default document name: index.html
- Optionally, enter error document path: 404.html
- Click *Save*

Azure creates a *$web* container for hosting.

---

### 3. *Upload Static Files*

- Go to *Containers > $web*
- Click *Upload*
- Select index.html, style.css, and other files from your project directory
- Click *Upload*

---

### 4. *Access Your Website*

- After uploading, go back to *Static Website* settings
- Copy the *Primary endpoint URL*
- Paste it in the browser to view your hosted static site.

Example:

https://<storage_account_name>.z13.web.core.windows.net


---

## 🧪 Example Files

### index.html
html
<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8">
  <title>My Azure Static Site</title>
  <link rel="stylesheet" href="style.css">
</head>
<body>
  <h1>Welcome to My Azure Website</h1>
  <p>This website is hosted on Azure Blob Storage!</p>
</body>
</html>


### style.css
css
body {
  font-family: Arial, sans-serif;
  background-color: #f4f4f4;
  text-align: center;
  padding: 50px;
}


---

## 📦 Folder Structure


azure-static-website/
├── index.html
├── style.css
└── 404.html (optional)


---

## 🔐 Security Considerations

- This website is *publicly accessible* by default.
- Avoid uploading sensitive data.
- You can use *Azure CDN* or *Custom Domain + HTTPS* for production usage.

---

## 🧠 Learning Outcomes

- Understanding Azure Storage Accounts and Blob service
- Hosting a website using cloud infrastructure
- Basic cloud deployment workflow

---

## 📈 Possible Extensions

- Add a *Contact Form* using Azure Functions (serverless backend)
- Deploy a *Portfolio Website*
- Connect a *Custom Domain* via Azure DNS
- Use *GitHub Actions* to automate deployment on file changes

---

## 📝 References

- [Azure Static Website Docs](https://learn.microsoft.com/en-us/azure/storage/blobs/storage-blob-static-website)
- [Azure Free Tier](https://azure.microsoft.com/en-us/free/)

---
