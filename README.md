# 🍽️ Restaurant Ordering System Demo

A modern Node.js + Express demo for restaurant ordering, staff management, and real-time payment with QR code support.

---

## 🚀 Quick Start

1. **Clone the repo**
   ```bash
   git clone https://github.com/yourusername/restaurant-demo.git
   cd restaurant-demo/prototype
   ```

2. **Install dependencies**
   ```bash
   npm install
   ```

3. **Run the server**
   ```bash
   npm start
   ```

---

## 👨‍🍳 Staff Panel

- **Access:**  
  Go to `/staff`, `/serve`, `/cashier` for staff operations.
- **Features:**  
  - View all orders in real time.
  - See what needs to be served.
  - Mark orders as served.
  - Access cashier for payment management.
  - View complete order history (`/order-history`).

---

## 🧑‍💼 Customer Ordering

- **Access:**  
  Open the main page (`/`) with a `table_id` in the URL, e.g.:
  ```
  http://localhost:3000/?table_id=1
  ```
  If no `table_id` is provided, the system will default to `0`.

- **Features:**  
  - Browse food categories and menus.
  - Add items to cart.
  - Place orders for your table.
  - View your order history and payment status.

---

## 💸 Payment Flow

- **QR Code Payment:**  
  - On the payment page, choose "QR Code PromptPay".
  - Scan the generated QR code with your mobile device.
  - After scanning, the system marks your payment as complete in real time and shows a fancy popup.
  - The payment page will automatically redirect or close when payment is confirmed.

- **Cashier Payment:**  
  - Choose "Pay at Cashier" on the payment page.
  - Go to the cashier desk to complete your payment.
  - Staff can mark your payment as complete from the staff panel.

---

## ⚡ Real-Time Features

- All order and payment updates are pushed instantly to staff and customer screens using Socket.io.
- Staff and customers see live status changes without refreshing.

---

## 🛠️ Developer Notes

- **Demo Mode:**  
  If `table_id` is missing, the app will auto-assign `0` and update the URL.
- **Security:**  
  QR payments use server-side validation to prevent fake payments.
- **Customization:**  
  You can change food categories, menu items, and images in the `/categories` folder.

---

## 📸 Screenshots

![Customer Menu](screenshots/menu.png)
![Staff Orders](screenshots/staff_orders.png)
![QR Payment](screenshots/qr_payment.png)

---

## 📝 License

MIT

---

**Enjoy your demo! If you have questions or want to contribute, open an issue or pull request.**
