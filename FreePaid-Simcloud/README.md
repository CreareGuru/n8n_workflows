# n8n-nodes-simcloud-freepaid

![image](https://github.com/user-attachments/assets/84793696-6dd0-421f-9b6c-78a5587b8055) ![image](https://github.com/user-attachments/assets/55e5a308-05a9-4ec9-ad6a-ab29ff68cf18) ![image](https://github.com/user-attachments/assets/dd473050-ff5d-4670-b4e0-336e2bc5d3b5)


** Documentation a work in progress **

** More Workflows for pinned requests to follow **

This custom set of workflows for [n8n](https://n8n.io) provides integration with the [Freepaid | Simcloud SOAP-based API](https://simcloud.co.za/aff/5078972) used for airtime-related operations.

## 📦 Features

- 🔐 Credential-based authentication (User ID & Password)
- 🧾 Four SOAP-based operations:
  - `fetchBalance`: Check your balance
  - `fetchProducts`: Get available products (e.g., airtime bundles)
  - `placeOrder`: Place an airtime/data order (pinless)
  - `queryOrder`: Query the status of an existing order
 
![image](https://github.com/user-attachments/assets/74b2d389-fe42-4bdc-b8e2-a1435f38fd75)

 - Note: Use https://ws.freepaid.co.za/airtimeplus/ instead of https://ws.test.freepaid.co.za/airtimeplus/

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

#### Links

[ws.freepaid.test.co.za/airtimeplus](https://ws.test.freepaid.co.za/airtimeplus/#)

[Freepaid PHP examples & Error Codes](https://ws.test.freepaid.co.za:443/airtimeplus/sample.html)

---

📝 License
MIT © [CreareGuru - www.creare.guru]
