# 🤖 Automated Math Quiz System with AI & Performance Tracking

As a Support Engineer, I believe the best way to handle repetitive tasks is to automate them out of existence. This project is a production-ready **n8n workflow** that generates daily math curriculum, delivers interactive quizzes via email, and automatically grades results.

## 🚀 Key Features
* **AI-Powered Content:** Integrates **Google Gemini** to dynamically generate math questions.
* **Custom Form Engine:** Uses a JavaScript Code Node to programmatically build an HTML form.
* **Robust Assessment Logic:** Features a custom grading algorithm that uses **Regex** to extract and compare numerical values.
* **Feedback Loop:** Automatically records performance data back to **Google Sheets**.

---

## 🛠️ Technical Deep Dive
### The "Test vs. Production" Webhook Challenge
A common hurdle in n8n is that Webhook nodes behave differently in test modes compared to production. I implemented a **data normalization layer** using a JavaScript Code Node to ensure that whether the webhook receives a single object (Production) or an array (Test), the downstream logic remains stable and doesn't break.

## 👨‍💻 Support Engineering Skills
* **API Integration:** Webhooks, Google OAuth2, and LLM connectivity.
* **Troubleshooting:** Solving environment-specific data structure mismatches.
* **Automation:** Reducing manual overhead for educational workflows.
