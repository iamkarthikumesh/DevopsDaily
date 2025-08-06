# Day 19 – Jenkins CI with Docker Agents

## 📹 Video Reference
**Course**: DevOps Zero to Hero by Abhishek Veeramalla  
**Day**: 19  
**YouTube Link**: [Watch here](https://www.youtube.com/watch?v=zZfhAXfBvVA)

---

## 🧠 Overview (What’s this day about?)
Learn how to set up **Jenkins pipelines** that use **Docker containers as agents** for isolated, consistent builds. You’ll understand how to run jobs in containers, configure agent labels, and structure multi-stage CI workflows.

---

## 🔧 Key Concepts & Commands

| Concept              | Description |
|----------------------|-------------|
| Jenkins Agents       | Use Docker containers as dynamic agents to run jobs |
| Declarative Pipeline | Define CI stages using the `Jenkinsfile` syntax |
| Docker Integration   | Jenkins can spin up Docker containers for each build stage |
| Jenkinsfile          | A script that defines pipeline logic (checkout, build, test, deploy) |

---

## 🗂 Files in this Folder

| File | Purpose |
|------|---------|
| `Jenkinsfile` | CI pipeline script for Jenkins |
| `docker-compose.yml` | Setup Jenkins master locally using Docker |
| `README.md` | Notes and explanations for this day |

---

## ✅ Step-by-Step Summary (Learn + Apply)

1. **Install Jenkins using Docker Compose**
2. **Configure Jenkins agent to use Docker**
3. **Write a Jenkinsfile for CI workflow**
4. **Run and troubleshoot builds in containers**
5. **Understand workspace and cleanup behavior**

---

## 📌 Practical Tips / Mistakes I Made

- 🔐 Docker agents need access to host Docker socket (`/var/run/docker.sock`)
- 🐳 Ensure your Jenkins user has permission to run Docker
- 🛠 Use unique agent labels to avoid job conflicts

---

## 📓 Notes to Self

- Use `docker exec -it jenkins bash` to debug container
- Always test Jenkinsfile syntax before committing (`pipeline syntax validator`)
- Clean up old workspaces to avoid Docker bloat

---

## 🤝 For Other Learners

If you're following along:
- Clone this folder
- Run the Jenkins Docker setup
- Modify the Jenkinsfile to fit your use-case
- Try breaking and fixing things — that’s how you learn!

---

