
# 🚀 DevOps Internship - Task 3: Infrastructure as Code (IaC) with Terraform

## 📌 Objective
Provision a local Docker container using **Terraform** to understand Infrastructure as Code (IaC) principles.

---

## 🧰 Tools Used
- [Terraform](https://www.terraform.io/)
- [Docker](https://www.docker.com/)

---

## 📂 Files Included
- `main.tf` – Terraform configuration file to provision the Docker container.
- `screenshots/` – (Optional) Folder for screenshots of terminal outputs.
- `README.md` – This documentation file.

---

## 🛠 Steps to Reproduce

### 1️⃣ Initialize Terraform
```bash
terraform init
```

### 2️⃣ Review Execution Plan
```bash
terraform plan
```

### 3️⃣ Apply Terraform Configuration
```bash
terraform apply -auto-approve
```

### 4️⃣ Check Running Container
```bash
docker ps
```
You should see an `nginx` container running on port `8080`.

### 5️⃣ List Terraform State
```bash
terraform state list
```

### 6️⃣ Destroy the Infrastructure
```bash
terraform destroy -auto-approve
```

---

## ⚙️ Terraform Configuration Details

- Pulls the `nginx:latest` image.
- Creates a container named `my-nginx`.
- Maps port `8080` on the host to port `80` in the container.

---

## 🌐 Output
Access the nginx container locally via:  
[http://localhost:8080](http://localhost:8080)

---
