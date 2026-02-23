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
🛠️ My Toolbox
💪 Core Skills (MERN & Beyond)
https://img.shields.io/badge/-React-61DAFB?logo=react&logoColor=white&style=flat
https://img.shields.io/badge/-Node.js-339933?logo=nodedotjs&logoColor=white&style=flat
https://img.shields.io/badge/-Express-000000?logo=express&logoColor=white&style=flat
https://img.shields.io/badge/-MongoDB-47A248?logo=mongodb&logoColor=white&style=flat
https://img.shields.io/badge/-JavaScript-F7DF1E?logo=javascript&logoColor=black&style=flat
https://img.shields.io/badge/-TypeScript-3178C6?logo=typescript&logoColor=white&style=flat
https://img.shields.io/badge/-HTML5-E34F26?logo=html5&logoColor=white&style=flat
https://img.shields.io/badge/-CSS3-1572B6?logo=css3&logoColor=white&style=flat
https://img.shields.io/badge/-Git-F05032?logo=git&logoColor=white&style=flat
https://img.shields.io/badge/-Postman-FF6C37?logo=postman&logoColor=white&style=flat

🧠 Currently Exploring (AI/ML Roadmap)
https://img.shields.io/badge/-Python-3776AB?logo=python&logoColor=white&style=flat
https://img.shields.io/badge/-PyTorch-EE4C2C?logo=pytorch&logoColor=white&style=flat
https://img.shields.io/badge/-LangChain-1C3C3C?logo=chainlink&logoColor=white&style=flat
https://img.shields.io/badge/-TensorFlow-FF6F00?logo=tensorflow&logoColor=white&style=flat
https://img.shields.io/badge/-HuggingFace-FFD21E?logo=huggingface&logoColor=black&style=flat
https://img.shields.io/badge/-MLOps-0078D4?logo=azuredevops&logoColor=white&style=flat

I'm still learning the depths of AI/ML, but I'm excited to apply them in real-world projects.

🔥 Featured Projects
Here are some of my best works – live demos and repositories.

📊 Kisanlog – Farmer Expense Tracker
A full-stack MERN application to help farmers log and analyze expenses, with a clean UI and backend on Render.
https://img.shields.io/badge/-Live%2520Demo-047857?style=flat&logo=render&logoColor=white
https://img.shields.io/badge/-GitHub%2520Repo-065f46?style=flat&logo=github&logoColor=white

👥 EMS – Employee Management System
A complete employee management solution built with the MERN stack, featuring CRUD operations and authentication.
https://img.shields.io/badge/-GitHub%2520Repo-065f46?style=flat&logo=github&logoColor=white

🛒 Two Good AU Clone
A pixel-perfect frontend clone of the "Two Good" website, showcasing responsive design and smooth animations.
https://img.shields.io/badge/-Live%2520Demo-047857?style=flat&logo=netlify&logoColor=white
https://img.shields.io/badge/-GitHub%2520Repo-065f46?style=flat&logo=github&logoColor=white

🌐 Personal Portfolio
My developer portfolio – built with React and hosted on Vercel.
https://img.shields.io/badge/-Live%2520Demo-047857?style=flat&logo=vercel&logoColor=white
https://img.shields.io/badge/-GitHub%2520Repo-065f46?style=flat&logo=github&logoColor=white
📊 GitHub Stats
https://github-readme-stats.vercel.app/api?username=Adinath-j&show_icons=true&theme=radical
https://github-readme-stats.vercel.app/api/top-langs/?username=Adinath-j&layout=compact&theme=radical
https://github-profile-summary-cards.vercel.app/api/cards/profile-details?username=Adinath-j&theme=radical
📈 Recent Activity
<!--RECENT_ACTIVITY:start--><!--RECENT_ACTIVITY:end--><!--RECENT_ACTIVITY:last_update-->
Last Updated: {{ date | relative }}

<!--RECENT_ACTIVITY:last_update_end-->
🌐 Connect With Me
https://img.shields.io/badge/-LinkedIn-0077B5?logo=linkedin&logoColor=white&style=flat
https://img.shields.io/badge/-GitHub-181717?logo=github&logoColor=white&style=flat
https://img.shields.io/badge/-Portfolio-047857?logo=vercel&logoColor=white&style=flat
https://img.shields.io/badge/-Email-D14836?logo=gmail&logoColor=white&style=flat (replace with your actual email if you want)

⭐ If you like my work, feel free to star some repositories – it means a lot!

---

## 🤖 Setting Up the GitHub Action for Recent Activity

To make the **Recent Activity** section update automatically, you need to add a workflow file to your profile repository.

1. In your `Adinath-j/Adinath-j` repo, create this folder: `.github/workflows/`
2. Inside it, create a file named `update-readme.yml` with the content below.
3. Commit and push the file. The action will run on a schedule (every 30 minutes) and after every push to your profile repo, updating the activity section.

```yaml
name: Update README with Recent Activity

on:
  schedule:
    - cron: '*/30 * * * *'  # every 30 minutes
  workflow_dispatch:        # allows manual trigger
  push:
    branches: [ main ]      # also runs when you push to main

jobs:
  update-readme:
    runs-on: ubuntu-latest
    steps:
      - uses: actions/checkout@v4
      - uses: jamesgeorge007/github-activity-readme@master
        with:
          GITHUB_TOKEN: ${{ secrets.GITHUB_TOKEN }}
          MAX_LINES: 10               # number of activities to show
          COMMIT_MSG: '⚡ Update recent activity'  # commit message
