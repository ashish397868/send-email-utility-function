# send-email-utility-function

A simple utility for sending emails using Node.js and Nodemailer. ✉️🚀

## 📦 Installation

```bash
npm install send-email-utility-function
```

## 🛠️ Usage

```javascript
const { sendEmail } = require('send-email-utility-function');

sendEmail({
  to: 'recipient@example.com',
  subject: 'Hello World',
  html: '<h1>Hello World</h1>',
}).then(info => {
  console.log('Email sent:', info.messageId);
}).catch(error => {
  console.error('Error sending email:', error);
});
```

## ⚙️ Environment Variables

Make sure to set the following environment variables:

- `EMAIL_USER`: Your email address 📧
- `EMAIL_PASSWORD`: Your email password or app password 🔑

## 🔑 How to Get a Gmail App Password

If you use Gmail, you need an **App Password** instead of your regular password. Here’s how to get one:

1. **Go to your Google Account**  
   👉 [Google Account](https://myaccount.google.com/)

2. **Enable 2-Step Verification**  
   🔒 Go to **Security** > **2-Step Verification**  
   🟢 Turn it ON (if not already enabled)

3. **Generate an App Password**  
   🔑 In **Security**, find **App passwords**  
   (You may need to sign in again)

4. **Create a new App Password**  
   ➕ Select **Mail** as the app  
   💻 Select your device (or choose "Other" and name it)

5. **Copy the 16-character password**  
   📋 Copy it and use it as your `EMAIL_PASSWORD` in your environment variables

⚠️ **Keep your app password safe!**  
You only need to enter it once in your `.env` file or environment settings.

---

## 📄 License

MIT