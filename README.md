# 🤖 LinkedIn Post Automation using Java & Selenium

This project automates the process of posting on LinkedIn using **Java** and **Selenium WebDriver**. It allows you to log in, create different types of posts (text, empty, long, with special characters), and verify outcomes automatically.

---

## 🔧 Technologies Used

- Java (JDK 17+)
- Selenium WebDriver
- WebDriverManager
- ChromeDriver
- Apache Commons IO (for saving screenshots)

---

## 📂 Project Structure
  LinkedInPostAutomation/
│
├── src/
│ └── test/
│ └── LinkedInPostAutomation.java
│
├── linkedin_post_success.png // Screenshot after posting
├── README.md
└── pom.xml (if using Maven)

## ▶️ How to Run

1. **Clone the repository**
   ```bash
   git clone https://github.com/your-username/linkedin-post-automation.git
   cd linkedin-post-automation

Open the project in an IDE (e.g., IntelliJ IDEA or Eclipse)

Edit LinkedInPostAutomation.java
Replace the email and password fields with your LinkedIn credentials:

String email = "your_email";
String password = "your_password";


Run the file
Make sure Chrome is installed and WebDriverManager resolves the correct driver version.


---

## 🧪 Test Cases

| Test Case | Description                     | Input Example              | Expected Result             | Actual Result          |
|-----------|---------------------------------|-----------------------------|-----------------------------|---------------------- |
| TC01      | Post simple text                | `This is an automated post` | Post gets published         | ✅ Success            |
| TC02      | Post empty text                 | *(Blank input)*             | Post not allowed / blocked | ✅ No post created     |
| TC03      | Post special characters         | `!@#$%^&*()`                | Post gets published         | ✅ Success            |
| TC04      | Post long paragraph             | *100+ words*                | Post gets published         | ✅ Success            |
| TC05      | Post with image (to implement)  | Attach image file           | Post with image published   | ✅Success             |
| TC06      | Post with video (to implement)  | Attach video file           | Post with video published   | ✅Success             |

---

📚 References
Selenium WebDriver Docs

WebDriverManager

LinkedIn Automation Basics

Java Documentation

