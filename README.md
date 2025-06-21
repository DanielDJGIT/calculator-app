# 🔢 Calculator Web Application

A simple, modern, and responsive calculator web app built using **HTML**, **CSS**, and **JavaScript**, deployed on an **AWS EC2 instance** using a CI/CD pipeline via **AWS CodePipeline, CodeBuild, and CodeDeploy**.

---

## 🚀 Features

- Stylish and responsive UI with gradient background
- Clickable number pad layout (0-9, ., +, −, ×, ÷, =, C)
- Clear input and instant result display
- Error handling for invalid expressions
- Fully automated deployment using GitHub and AWS services

---

## 🧾 Tech Stack

| Frontend     | CI/CD              | Cloud Infrastructure    |
|--------------|--------------------|--------------------------|
| HTML, CSS, JS| Git, CodePipeline  | AWS EC2, CodeBuild, CodeDeploy |

---

## 🛠️ Project Structure


---

## ⚙️ Setup & Deployment (CI/CD)

### 1. ✅ **Create GitHub Repository**
Push this code to your GitHub repository (e.g., `calculator-app`)

### 2. 🖥️ **Launch EC2 Instance**
- Amazon Linux 2, enable HTTP (port 80)
- Install and start CodeDeploy agent
- Tag instance with: `Name = CalculatorServer`

### 3. 🧠 **Create CodeDeploy App**
- Application: `CalculatorApp`
- Deployment Group: `CalcDeploymentGroup`

### 4. 🛠️ **CodeBuild Project**
- Connect GitHub repo
- Use buildspec.yml (even if dummy)
- Output artifacts: `**/*`

### 5. 🔁 **CodePipeline**
- Source: GitHub
- Build: CodeBuild
- Deploy: CodeDeploy

---

## 💡 Usage

Visit your deployed calculator using your EC2 public IP:

---

## 📷 Demo Screenshot

![Calculator Screenshot](https://your-screenshot-url.com/preview.png)

---

## 📦 Future Enhancements

- [ ] Add keyboard support
- [ ] Add calculation history
- [ ] Dark/light theme toggle
- [ ] PWA support for offline use

---

## 🙌 Acknowledgments

Built for learning AWS DevOps CI/CD automation and frontend fundamentals.

---

## 📜 License

This project is licensed under the [MIT License](LICENSE).

