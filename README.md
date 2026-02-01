# Image Upload Web App

This is a simple Flask-based web application that allows users to **upload** and **delete images**. It also includes an **IP whitelisting** feature to restrict access to a specific IP address.

---

## 🚀 Features

- Upload images (`.jpg`, `.jpeg`, `.png`, `.gif`)
- View uploaded images
- Delete images
- IP restriction using Flask middleware
- Simple and clean HTML interface

---

## 🔐 Access Control

Only requests from the IP address `20.218.226.24` are allowed to access the app.  
Other IPs will receive a `403 Forbidden` response.

> This check is handled in the `@app.before_request` section of `app.py`.

---

## 🛠 Setup Instructions

### 1. Clone the repository

```bash
git clone https://github.com/cyberalmamun/image-upload-app.git
cd image-upload-app
