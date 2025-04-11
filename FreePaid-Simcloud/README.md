# 🌩️ n8n-nodes-simcloud

This custom set of workflows for [n8n](https://n8n.io) provides integration with the [Freepaid | Simcloud SOAP-based API](https://simcloud.co.za/aff/5078972) used for airtime-related operations.

## 📦 Features

- 🔐 Credential-based authentication (User ID & Password)
- 🧾 Four SOAP-based operations:
  - `fetchBalance`: Check your balance
  - `fetchProducts`: Get available products (e.g., airtime bundles)
  - `placeOrder`: Place an airtime/data order (pinless)
  - `queryOrder`: Query the status of an existing order
 
![image](https://github.com/user-attachments/assets/74b2d389-fe42-4bdc-b8e2-a1435f38fd75)


---

## 🚀 Installation

Open workflow then top right of screen click the 3 dots and select "Import from File" then select the JSON file

## 🔑 Credentials

User ID: Your Freepaid account username

Password: Your Freepaid account password

---

## ⚙️ Available Operations

### 1. fetchBalance

Purpose: Retrieve your current account balance.

No additional parameters needed.

---

### 2. fetchProducts

Purpose: Fetch a list of available airtime/data products.

No additional parameters needed.

---

### 3. placeOrder

Purpose: Place an airtime/data order (e.g., pinless recharge).

#### Parameters:

refno (string): Reference number (e.g., order ID)

network (string): Product network code (e.g., p-vodacom)

sellvalue (string): Amount or denomination

count (number): Quantity (e.g., 1)

extra (string): Target phone number

---

### 4. queryOrder

Purpose: Get status of a previously placed order.

#### Parameters:

orderno (string): Order number (returned from placeOrder)

---

📝 License
MIT © [CreareGuru - www.creare.guru]
