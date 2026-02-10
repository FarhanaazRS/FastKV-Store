# 🚀 FastKV-Store

A high-performance in-memory Key-Value Store built using **ASP.NET Core** and **Microsoft FASTER**.  
This project exposes RESTful APIs to perform key-value operations, checkpointing, and recovery.

---

## 📌 Overview

FastKV-Store is a backend Web API that wraps Microsoft’s **FASTER** key-value engine and exposes it via HTTP endpoints.

It demonstrates:

- In-memory data storage
- High-performance key-value operations
- Checkpoint creation & recovery
- ASP.NET Core Web API architecture
- Clean service-based design

---

## 🛠 Tech Stack

- **ASP.NET Core**
- **C#**
- **Microsoft FASTER (Key-Value Engine)**
- **Swagger (OpenAPI)**
- **.NET 8 Runtime**

---

## 🏗 Project Architecture

```
FastKV-Store
│
├── Controllers       → API Endpoints
├── Services          → FASTER KV Logic
├── Models            → Request / Response Models
├── Startup.cs        → Dependency Injection & Middleware
└── Program.cs        → Application Entry Point
```

The service layer interacts with the FASTER engine, while controllers expose REST endpoints.

---

## ⚙️ How to Run Locally

### 1️⃣ Clone the repository

```bash
git clone https://github.com/FarhanaazRS/FastKV-Store.git
cd FastKV-Store/FastKV-Store
```

### 2️⃣ Install Required Runtime

Make sure you have:

- .NET 8 Runtime installed

Check:

```bash
dotnet --version
```

### 3️⃣ Run the application

```bash
dotnet run
```

### 4️⃣ Open Swagger UI

```
http://localhost:5000/swagger
```

---

## 📡 API Endpoints

### 🔹 Cars Controller

- `GET /api/Cars`
- `POST /api/Cars`
- `GET /api/Cars/{id}`

### 🔹 Testing Controller (KV Operations)

- `GET /api/Testing/GetStoredCollection`
- `GET /api/Testing/GetStoredCollection/{key}`
- `GET /api/Testing/CreateDemoCollection`
- `GET /api/Testing/CreateCheckpoint`
- `GET /api/Testing/RestoreCheckpoint`

---

## 🚀 Features

- In-memory high-speed KV storage
- Persistent checkpoint support
- RESTful API interface
- Modular and scalable backend structure
- Swagger API documentation

---

## 🧠 Learning Objectives

This project demonstrates:

- Backend service design in ASP.NET Core
- Working with high-performance storage engines
- Handling application lifecycle & background services
- Building and testing APIs using Swagger

---

## 💼 Resume Description

Built a high-performance in-memory Key-Value Store using ASP.NET Core and Microsoft FASTER with checkpointing and REST API integration.

---

## 📜 License

This project is for educational and learning purposes.
