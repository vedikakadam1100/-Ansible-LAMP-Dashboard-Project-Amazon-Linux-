# 🚀 Ansible LAMP Dashboard Project (Amazon Linux)

A **GitHub-ready DevOps project** that automates the deployment of a **LAMP stack** (Apache, MariaDB, PHP) on **Amazon Linux** using **Ansible**, and serves a **custom PHP Server Status Dashboard**.

---

## 📌 Project Highlights

* ✅ Fully automated LAMP stack setup
* ✅ Amazon Linux compatible
* ✅ Modern PHP-based Server Dashboard UI
* ✅ Uses Ansible best practices (variables, loops)
* ✅ Interview & portfolio ready

---

## 🧱 Tech Stack

* **Ansible** – Configuration Management
* **Apache (httpd)** – Web Server
* **MariaDB** – Database Server
* **PHP + PHP-FPM** – Backend
* **Amazon Linux** – Target OS

---

## 📂 Project Structure

```bash
ansible-lamp-dashboard/
│
├── inventory
├── ansible.cfg
├── lamp_dashboard.yml
├── README.md
└── screenshots/
    └── dashboard-output.png
```

---

## ⚙️ Configuration Files

### 🔹 inventory

```ini
[lamp]
localhost ansible_connection=local
```

### 🔹 ansible.cfg

```ini
[defaults]
inventory = inventory
host_key_checking = False
```

---

## ▶️ Main Playbook

**File:** `lamp_dashboard.yml`

This playbook:

* Installs Apache, MariaDB, PHP, PHP-FPM
* Starts and enables all services
* Deploys a custom PHP dashboard website

Run using:

```bash
ansible-playbook lamp_dashboard.yml
```

---

## 🌐 Application Output

Once playbook execution completes, open browser:

```text
http://<EC2-PUBLIC-IP>/
```

### Dashboard Shows:

* Server status (ONLINE)
* PHP version
* Hostname
* Server IP
* Current date & time

---

## 🖼 Screenshots

![](./img/Screenshot%202025-12-21%20190230.png)

![](./img/Screenshot%202025-12-21%20190414.png)

![](./img/Screenshot%202025-12-21%20190138.png)

---

## 💼 Resume / Interview Description

> Automated deployment of LAMP stack on Amazon Linux using Ansible. Built a custom PHP-based server dashboard displaying real-time system information. Project follows Infrastructure as Code and automation best practices.

---

## 🧠 Key Learnings

* Ansible playbook design
* Package & service automation
* PHP deployment via Ansible
* Amazon Linux service handling

---

## 👩‍💻 Author

**Vedika Kadam**
DevOps | Cloud | Automation

---

## ⭐ How to Use

1. Clone the repo
2. Ensure Ansible is installed
3. Run the playbook
4. Access the dashboard via browser

---

## 📌 License

This project is for learning and portfolio purposes.

---
