# 🐳 Jenkins Pipeline with Docker Agent (Node.js Example)

This guide shows how to configure **Jenkins** to run a pipeline using a **Docker container as the agent**, specifically with the `node:16-alpine` image.

---

## 👥 Add Users to Docker Group

Make sure both `jenkins` and `ubuntu` users can access Docker:

```bash
sudo usermod -aG docker jenkins
sudo usermod -aG docker ubuntu
