# 📱 Twilio-Based Automated WhatsApp Notification System

This is a **Python-based CLI application** that automates sending personalized WhatsApp messages to multiple recipients at a **scheduled future date and time**. It leverages the **Twilio WhatsApp API** to deliver reliable and customized notifications.

---

## 🚀 Features

- ✅ Collect multiple recipients with custom messages  
- ✅ Schedule messages for a specific date and time  
- ✅ Automatic delay calculation until send time  
- ✅ Personalized content using recipient names  
- ✅ Real-time status updates and error handling  
- ✅ Lightweight CLI app – no server or database needed

---

## 🔧 How It Works

### 1. Input Recipients

- User enters **name**, **WhatsApp number**, and a **custom message**  
- Repeats until all recipients are added

### 2. Schedule Message

- Enter target date (`YYYY-MM-DD`) and time (`HH:MM`, 24-hour format)

### 3. Wait Until Scheduled Time

- Script calculates the delay and pauses execution

### 4. Send Messages

- Sends each message via Twilio’s WhatsApp API  
- Logs message SID or any errors

---

## 📦 Requirements

- Python 3.6+
- Twilio account with WhatsApp sandbox enabled
- Twilio Python library

---

## 💻 Installation

```bash
git clone https://github.com/yourusername/whatsapp-scheduler.git
cd whatsapp-scheduler
pip install twilio
```

---

## 🔑 Configuration

Edit the script and replace with your Twilio credentials:

```python
account_sid = 'YOUR_ACCOUNT_SID'
auth_token = 'YOUR_AUTH_TOKEN'
from_whatsapp_number = 'whatsapp:+14155238886'  # Twilio sandbox number
```

---

## ▶ Usage

Run the script using:

```bash
python whatsapp_scheduler.py
```

Follow the interactive CLI to:

- Add multiple recipients and custom messages
- Set the schedule
- Automatically send messages at the right time

---

## ⚠ Notes

- **Twilio Trial**: Only verified numbers can receive messages in sandbox mode  
- **For Production**: Upgrade Twilio and request WhatsApp Business API access  
- **Security Tip**: Never expose your `auth_token`. Use environment variables or a `.env` file.

---

## 📄 License

This project is open-source and available under the **MIT License**.

---

## 🙌 Acknowledgments

- [Twilio WhatsApp API Documentation](https://www.twilio.com/docs/whatsapp)

---

## 📬 Contact

Made with ❤️ by **Sravya Reddy**

- 📧 Email: salvendrisravyareddy@gmail.com  
- 💼 LinkedIn: [Sravya Reddy](https://www.linkedin.com/in/sravya-reddy-545632265/)
