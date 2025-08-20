📧 Universal Email Verification API









A free, open-source email verification API built with Node.js, MongoDB, and Gmail.
Deployable on Vercel and usable on all your websites.


---

✨ Features

✅ Free & fast email verification

✅ Works with all websites (frontend can be HTML, React, etc.)

✅ Sends 6-digit verification codes via Gmail

✅ Secure: codes expire after 15 minutes

✅ Ready for Vercel deployment

✅ Uses MongoDB Atlas (cloud DB)



---

🚀 Quick Start

1. Clone repo

git clone https://github.com/YOURNAME/verify-api.git
cd verify-api

2. Install dependencies

npm install

3. Setup .env

Create .env in the project root:

MONGO_URI=your_mongodb_atlas_uri
GMAIL_USER=yourgmail@gmail.com
GMAIL_PASS=your_app_password   # from Google App Passwords

👉 Generate Gmail app password here: Google App Passwords

4. Run locally

npm run dev

Now open http://localhost:3000

5. Deploy to Vercel

Push project to GitHub

Import into Vercel

Add environment variables in Project Settings → Environment Variables

Deploy 🚀


Or just click this 👇



---

🔑 API Endpoints

POST /api/send-code

Send a 6-digit code to email.

{ "email": "user@example.com" }

Response:

{ "success": true, "message": "Code sent" }


---

POST /api/verify-code

Verify code.

{ "email": "user@example.com", "code": "123456" }

Response:

{ "success": true, "message": "Email verified!" }


---

🌍 Example Frontend Integration

<script>
async function sendCode() {
  const res = await fetch("https://tcroneb.vercel.app/api/send-code", {
    method: "POST",
    headers: { "Content-Type": "application/json" },
    body: JSON.stringify({ email: "user@example.com" })
  });
  console.log(await res.json());
}
</script>


---

💖 Support Development

This project is free & open source 🎉

If you find it useful, consider donating:
👉 Donate here


---

👨‍💻 Created By World of Technology ⁴⁰³ TeaM

Built with ❤️ by Tcroneb Hackx

Free to use for personal & commercial projects

MIT License



---

📜 License

This project is licensed under the MIT License – free to use, modify, and distribute.
