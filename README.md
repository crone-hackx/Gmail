<h1 align="center">📧 Universal Email Verification API</h1>

<p align="center">
  <img src="https://img.shields.io/badge/License-MIT-green.svg" />
  <img src="https://img.shields.io/badge/Node.js-18+-blue?logo=node.js" />
  <img src="https://img.shields.io/badge/Database-MongoDB-green?logo=mongodb" />
  <img src="https://img.shields.io/badge/Deploy-Vercel-black?logo=vercel" />
  <img src="https://img.shields.io/badge/Status-Free%20%26%20Open%20Source-brightgreen" />
</p>

<p align="center">
  <a href="https://vercel.com/new/clone?repository-url=https://github.com/YOURNAME/verify-api&project-name=verify-api&repository-name=verify-api">
    <img src="https://vercel.com/button" alt="Deploy with Vercel"/>
  </a>
</p>

---

## ✨ About

🚀 A free, open-source **email verification API** built with **Node.js, MongoDB Atlas, and Gmail**.  
Use it to send **6-digit verification codes** for signup, login, or user validation.  

<p align="center">
  <img src="https://media.giphy.com/media/hqU2KkjW5bE2v2Z7Q2/giphy.gif" width="400" alt="Email animation"/>
</p>

---

## ⚡ Features
- ✅ Works on **all your websites** (HTML, React, Next.js, etc.)  
- ✅ Free Gmail sender (via App Password)  
- ✅ Secure → codes expire after **15 minutes**  
- ✅ Deployed as **serverless API** on Vercel  
- ✅ Auto-deploy with **GitHub Actions**  

---

## 🚀 Quick Start

### 1️⃣ Clone repo
```bash
git clone https://github.com/YOURNAME/verify-api.git
cd verify-api

2️⃣ Install dependencies

npm install

3️⃣ Setup .env

MONGO_URI=your_mongodb_atlas_uri
GMAIL_USER=yourgmail@gmail.com
GMAIL_PASS=your_app_password   # from Google App Passwords

👉 Generate Gmail app password here: Google App Passwords

4️⃣ Run locally

npm run dev

Open http://localhost:3000

5️⃣ Deploy to Vercel

Push repo to GitHub

Import into Vercel

Add Environment Variables (MONGO_URI, GMAIL_USER, GMAIL_PASS)

Deploy 🚀


Or just click this 👇

<p>
  <a href="https://vercel.com/new/clone?repository-url=https://github.com/YOURNAME/verify-api&project-name=verify-api&repository-name=verify-api">
    <img src="https://vercel.com/button" alt="Deploy with Vercel"/>
  </a>
</p>
---

🔑 API Endpoints

📤 POST /api/send-code

{ "email": "user@example.com" }

✅ Sends a code to email


---

📥 POST /api/verify-code

{ "email": "user@example.com", "code": "123456" }

✅ Verifies code & marks user as verified


---

##🌍 Example Frontend Integration

<script>
async function sendCode() {
  const res = await fetch("https://yourproject.vercel.app/api/send-code", {
    method: "POST",
    headers: { "Content-Type": "application/json" },
    body: JSON.stringify({ email: "user@example.com" })
  });
  console.log(await res.json());
}
</script>
</div>



##💖 Support Development

This project is free & open source 🎉
If you find it useful, consider supporting me:

<p align="center">
  <a href="https://tcroneb.qzz.io/donate" target="_blank">
    <img src="https://img.shields.io/badge/💖%20Donate-Support%20this%20project-pink?style=for-the-badge" alt="Donate Button"/>
  </a>
</p>


👨‍💻 Created By World of Technology 4⁰3 Team

Built with ❤️ by Tcroneb Hackx 

Free for personal & commercial projects

MIT License



---

📜 License

Licensed under the MIT License – free to use, modify, and share.
