# Inventory Tracking System

This is a simple Inventory Tracking System built using **Node.js**, **Express**, and **SQLite** to manage stock movements.

## 🚀 Features
- Record inventory movements (Stock In, Sale, Manual Removal, Adjustment)
- Validate stock levels before sales
- Maintain transaction history

## 🛠️ Setup Instructions

### 1️⃣ Clone the Repository
```sh
git clone https://github.com/mibma/inventory-stage1.git
cd inventory-stage1
```

### 2️⃣ Install Dependencies
```sh
npm install
```

### 3️⃣ Initialize SQLite Database
```sh
sqlite3 inventory.db < schema.sql
```

### 4️⃣ Start the Server
```sh
node server.js
```

Server runs on **http://localhost:3000**.

## 📌 API Endpoints

### **1️⃣ Record Stock Movement**
**POST** `/inventory/movement`

#### **Request Body:**
```json
{
  "product_id": 1,
  "quantity_change": 10,
  "movement_type": "STOCK_IN",
  "reference_id": "Ref123",
  "notes": "Initial Stock"
}
```

#### **Response:**
```json
{
  "message": "Inventory updated successfully",
  "movement_id": 1
}
```

## 📝 License
This project is open-source under the **MIT License**.

---
Made with ❤️ by **@mibma**

