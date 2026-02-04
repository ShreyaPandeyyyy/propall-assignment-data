# 📦 Propall Assignment — Cloud JSON Data Source

This repository hosts the **cloud JSON data** used by the Propall full-stack assignment.

Instead of storing user and role data inside the backend, the server fetches these files **directly from GitHub Raw URLs**, simulating a real production scenario where data is stored in a remote cloud source.

---

## 📁 Files

| File         | Purpose                                      |
|--------------|-----------------------------------------------|
| `users.json` | Stores user records displayed in dashboard   |
| `roles.json` | Stores role-based access (admin / viewer)    |

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
```

---

## 🚀 What this proves in the assignment

This setup demonstrates:

- Use of external cloud-hosted data sources
- Real-time dashboard updates using Socket.io
- Separation of data layer from application layer
- Role-based access using remote JSON configuration
- Practical full-stack architecture similar to production systems

---

## 👩‍💻 Author

**Shreya Pandey**  
B.E. Electronics & Communication Engineering  
BMS College of Engineering
