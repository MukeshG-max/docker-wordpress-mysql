# WordPress + MySQL with Docker Compose

A fully containerized WordPress site backed by MySQL, deployed using Docker Compose.  

---

## 📌 What This Project Does

- Runs **WordPress** (web app) and **MySQL** (database) as separate containers
- Containers communicate via a custom Docker **network**
- MySQL data **persists** even if containers restart (Docker Volumes)
- Entire stack launches with a **single command**

---

## 🧱 Architecture

```
Browser
   │
   ▼
WordPress Container (port 8080)
   │  (wp-network)
   ▼
MySQL Container
   │
   ▼
mysql-data Volume (persistent storage)
```

---

## 🛠️ Tech Stack

| Tool | Purpose |
|---|---|
| Docker | Containerization |
| Docker Compose | Multi-container orchestration |
| WordPress | Web application |
| MySQL 8.0 | Database |

---

## 🚀 How to Run

### Prerequisites
- Docker installed
- Docker Compose installed

### Steps

```bash
# 1. Clone this repo
git clone https://github.com/YOURUSERNAME/docker-wordpress-mysql.git
cd docker-wordpress-mysql

# 2. Start the containers
docker-compose up -d

# 3. Open in browser
http://localhost:8080
```

### Stop the containers
```bash
docker-compose down
```

### Stop and delete all data
```bash
docker-compose down -v
```

---

## 📁 Project Structure

```
docker-wordpress-mysql/
└── docker-compose.yml     # Full stack definition
└── README.md              # This file
```

---

## 📚 What I Learned

- How to write a `docker-compose.yml` file
- Connecting containers using Docker networks
- Persisting data using Docker volumes
- Deploying a multi-container application
- How WordPress and MySQL communicate in production-style 

---

## 👤 Author

**Mukesh G**  
[LinkedIn](https://www.linkedin.com/in/mukesh-g-6b9592269) • [GitHub](https://github.com/MukeshG-max)
