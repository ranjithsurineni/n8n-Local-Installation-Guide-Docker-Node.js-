# 🚀 n8n Local Installation Guide (Docker & Node.js)

This guide will help you install and run **n8n**, the popular workflow automation tool, on your **local machine** using either:

- Docker (Recommended for ease)
- Node.js (For developers who prefer npm-based setup)

---

## 📦 Prerequisites

- Docker & Docker CLI installed: [Install Docker](https://www.docker.com/products/docker-desktop)
- Node.js (if using the manual method): [Install Node.js](https://nodejs.org/)

---

## 🔧 Method 1: Run n8n using Docker (RECOMMENDED)

### 🧹 Step 1: Clean Existing Docker Resources (Optional)

Before starting fresh:

```bash
docker stop $(docker ps -aq)
docker rm $(docker ps -aq)
docker system prune -a -f
```

🚀 Step 2: Run n8n in a Container

```bash
docker run -d --name n8n_instance -p 5678:5678 n8nio/n8n
```

✅ Step 4: Access n8n in Browser

visit:
```bash
http://localhost:5678
```
or
```bash
http://127.0.0.1:5678
```

**You should now see the n8n workflow UI! 🎉**


=======================================================
## 🧑‍💻 Method 2: Run n8n using Node.js (Without Docker)

📦 Step 1: Install n8n globally
```bash
npm install n8n -g
```

▶️ Step 2: Start n8n
```bash
n8n
```

By default, this starts n8n on:

```bash
http://localhost:5678
```

If needed, you can change the port:

```bash
n8n --port=8080
```

## 🧠 About n8n

n8n is an extendable workflow automation tool that lets you connect APIs, services, and custom logic — no code needed!

Explore more at: https://n8n.io

=====================================

🏁 Get Started Building Workflows Today!

If this helped, ⭐️ the repo or fork it to share with your team.
