# 📦 Propall Assignment — Cloud JSON Data Source

This repository hosts the **cloud JSON data** used by the Propall full-stack assignment.

Instead of storing user and role data inside the backend, the server fetches these files **directly from GitHub Raw URLs**, simulating a real production scenario where data is stored in a remote cloud source.

---

## 📁 Files

| File         | Purpose                                   |
|--------------|--------------------------------------------|
| `users.json` | Stores user records displayed in dashboard |
| `roles.json` | Stores role-based access (admin / viewer)  |

---

## 🎯 Why this repository exists

This setup demonstrates a **real-world architecture** where:

- Data is fetched from a remote cloud source
- The server consumes external JSON APIs
- Services rely on external data providers
- Role-based access is controlled using hosted data

Instead of keeping data inside the backend, this project shows **decoupled architecture**.

---

## 🧠 Architecture Flow

```text
GitHub JSON (Cloud Data)
        ↓
Express Server (fetches data using RAW URLs)
        ↓
Socket.io broadcasts updates
        ↓
Next.js Client Dashboard updates in real-time
