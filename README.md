# 📰 WhatsApp News Bot

This Python automation project sends real-time news updates about the **India-Pakistan conflict** to a WhatsApp number every hour. It uses **NewsAPI** to fetch the news and **Twilio WhatsApp API** to send the messages.

---

## 🔗 APIs Used

1. **NewsAPI**  
   - 📌 Used to fetch news articles  
   - 🌐 Website: [https://newsapi.org](https://newsapi.org)

2. **Twilio WhatsApp API**  
   - 📌 Used to send WhatsApp messages  
   - 🌐 Website: [https://www.twilio.com/whatsapp](https://www.twilio.com/whatsapp)

---

## 🔐 How to Get API Keys

### 🔹 NewsAPI Key:
- Visit [https://newsapi.org/register](https://newsapi.org/register)
- Sign up and log in
- Copy the API key from your dashboard

### 🔹 Twilio Credentials:
- Go to [https://www.twilio.com/whatsapp](https://www.twilio.com/whatsapp)
- Sign up and verify your number
- Set up a project
- Copy your:
  - **Account SID**
  - **Auth Token**
  - Use the default sandbox number: `whatsapp:+14155238886`

---

## 🧰 Tech Stack Used

| Technology       | Purpose                            |
|------------------|------------------------------------|
| Python           | Core programming language          |
| Requests         | To make HTTP calls to NewsAPI      |
| Twilio SDK       | To send WhatsApp messages          |
| Time             | For scheduling the hourly task     |

---

## 🔄 Automation Frequency

- The bot runs in an infinite loop using `while True`
- It sends an update every **1 hour** using:  
  ```python
  time.sleep(3600)
