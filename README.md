# 👋 Hey, I'm **Adinath Jadhav**

I build systems that combine **software engineering + artificial intelligence + product thinking**.  
My long-term goal is to design **human-centered AI platforms**, not just apps.

---

## 🧑‍💻 About Me

```ts
const adinath = {
  name: "Adinath Jadhav",
  role: "Aspiring AI Engineer & Full-Stack Developer",
  core_stack: ["React", "Node.js", "Express", "MongoDB", "TypeScript"],
  currently_working_on: "Dynamic Developer Homepage Extension",
  currently_learning: ["TypeScript", "AI/ML", "System Design"],
  goals: [
    "Build my own AI system",
    "Create innovative developer tools"
  ]
}
```

### 🛠️ My Toolbox

#### 💪 Core Skills (MERN & Beyond)

![React](https://img.shields.io/badge/-React-61DAFB?logo=react&logoColor=white&style=flat)
![Node.js](https://img.shields.io/badge/-Node.js-339933?logo=nodedotjs&logoColor=white&style=flat)
![Express](https://img.shields.io/badge/-Express-000000?logo=express&logoColor=white&style=flat)
![MongoDB](https://img.shields.io/badge/-MongoDB-47A248?logo=mongodb&logoColor=white&style=flat)
![JavaScript](https://img.shields.io/badge/-JavaScript-F7DF1E?logo=javascript&logoColor=black&style=flat)
![TypeScript](https://img.shields.io/badge/-TypeScript-3178C6?logo=typescript&logoColor=white&style=flat)
![HTML5](https://img.shields.io/badge/-HTML5-E34F26?logo=html5&logoColor=white&style=flat)
![CSS3](https://img.shields.io/badge/-CSS3-1572B6?logo=css3&logoColor=white&style=flat)
![Git](https://img.shields.io/badge/-Git-F05032?logo=git&logoColor=white&style=flat)
![Postman](https://img.shields.io/badge/-Postman-FF6C37?logo=postman&logoColor=white&style=flat)

#### 🧠 Currently Exploring (AI/ML Roadmap)

![Python](https://img.shields.io/badge/-Python-3776AB?logo=python&logoColor=white&style=flat)
![PyTorch](https://img.shields.io/badge/-PyTorch-EE4C2C?logo=pytorch&logoColor=white&style=flat)
![LangChain](https://img.shields.io/badge/-LangChain-1C3C3C?logo=chainlink&logoColor=white&style=flat)
![TensorFlow](https://img.shields.io/badge/-TensorFlow-FF6F00?logo=tensorflow&logoColor=white&style=flat)
![Hugging Face](https://img.shields.io/badge/-HuggingFace-FFD21E?logo=huggingface&logoColor=black&style=flat)
![MLOps](https://img.shields.io/badge/-MLOps-0078D4?logo=azuredevops&logoColor=white&style=flat)

I'm still learning the depths of AI/ML, but I'm excited to apply them in real-world projects.

---

## 🔥 Featured Projects

Here are some of my best works – live demos and repositories.

### 📊 Kisanlog – Farmer Expense Tracker

A full-stack MERN application to help farmers log and analyze expenses, with a clean UI and backend on Render.

[![Live Demo](https://img.shields.io/badge/-Live%20Demo-047857?style=flat&logo=render&logoColor=white)](https://kisanlogwbackend.onrender.com/)
[![GitHub Repo](https://img.shields.io/badge/-GitHub%20Repo-065f46?style=flat&logo=github&logoColor=white)](https://github.com/Adinath-j/Kisanlog)

### 👥 EMS – Employee Management System

A complete employee management solution built with the MERN stack, featuring CRUD operations and authentication.

[![GitHub Repo](https://img.shields.io/badge/-GitHub%20Repo-065f46?style=flat&logo=github&logoColor=white)](https://github.com/Adinath-j/EMS-Employee-Management-System)

### 🛒 Two Good AU Clone

A pixel-perfect frontend clone of the "Two Good" website, showcasing responsive design and smooth animations.

[![Live Demo](https://img.shields.io/badge/-Live%20Demo-047857?style=flat&logo=netlify&logoColor=white)](https://two-good-au.netlify.app/)
[![GitHub Repo](https://img.shields.io/badge/-GitHub%20Repo-065f46?style=flat&logo=github&logoColor=white)](https://github.com/Adinath-j/two-good-au)

### 🌐 Personal Portfolio

My developer portfolio – built with React and hosted on Vercel.

[![Live Demo](https://img.shields.io/badge/-Live%20Demo-047857?style=flat&logo=vercel&logoColor=white)](https://portfolio2-flame-psi.vercel.app/)
[![GitHub Repo](https://img.shields.io/badge/-GitHub%20Repo-065f46?style=flat&logo=github&logoColor=white)](https://github.com/Adinath-j/portfolio2)

---

## 📊 GitHub Stats

![GitHub Stats](https://github-readme-stats.vercel.app/api?username=Adinath-j&show_icons=true&theme=radical)

![Top Languages](https://github-readme-stats.vercel.app/api/top-langs/?username=Adinath-j&layout=compact&theme=radical)

![Profile Summary](https://github-profile-summary-cards.vercel.app/api/cards/profile-details?username=Adinath-j&theme=radical)

---

## 📈 Recent Activity

<!--RECENT_ACTIVITY:start-->
<!--RECENT_ACTIVITY:end-->
<!--RECENT_ACTIVITY:last_update-->
Last Updated: {{ date | relative }}
<!--RECENT_ACTIVITY:last_update_end-->

---

## 🌐 Connect With Me

[![LinkedIn](https://img.shields.io/badge/-LinkedIn-0077B5?logo=linkedin&logoColor=white&style=flat)](https://www.linkedin.com/in/adinath-jadhav)
[![GitHub](https://img.shields.io/badge/-GitHub-181717?logo=github&logoColor=white&style=flat)](https://github.com/Adinath-j)
[![Portfolio](https://img.shields.io/badge/-Portfolio-047857?logo=vercel&logoColor=white&style=flat)](https://portfolio2-flame-psi.vercel.app/)
[![Email](https://img.shields.io/badge/-Email-D14836?logo=gmail&logoColor=white&style=flat)](mailto:adinath.j@example.com)

> 💡 **Note:** Replace the email link with your actual email address.

⭐ If you like my work, feel free to star some repositories – it means a lot!

---

## 🤖 Setting Up the GitHub Action for Recent Activity

To make the **Recent Activity** section update automatically, you need to add a workflow file to your profile repository.

1. In your `Adinath-j/Adinath-j` repo, create this folder: `.github/workflows/`
2. Inside it, create a file named `update-readme.yml` with the following content:

```yaml
name: Update README with Recent Activity

on:
  schedule:
    - cron: '*/30 * * * *'  # Run every 30 minutes
  push:
    branches:
      - main
  workflow_dispatch:  # Allow manual trigger

jobs:
  update-readme:
    runs-on: ubuntu-latest
    steps:
      - name: Checkout repository
        uses: actions/checkout@v3
        with:
          fetch-depth: 0

      - name: Update README with recent activity
        uses: jamesgeorge007/github-activity-readme@master
        env:
          GITHUB_TOKEN: ${{ secrets.GITHUB_TOKEN }}
        with:
          COMMIT_MSG: '⚡ Update recent activity'
          MAX_LINES: 10

      - name: Commit and push changes
        run: |
          git config user.name "GitHub Action"
          git config user.email "action@github.com"
          git add README.md
          git commit -m "⚡ Update recent activity" --allow-empty
          git push
```

3. Commit and push the file. The action will run on a schedule (every 30 minutes) and after every push to your main branch, updating the activity section automatically.
