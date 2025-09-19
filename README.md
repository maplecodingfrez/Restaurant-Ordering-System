# Restaurant Ordering System Demo

---

## 🚀 Quick Start

1. **Clone the repo**
   ```bash
   git clone https://github.com/maplecodingfrez/restaurant-demo.git
   cd restaurant-demo
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

## Staff Panel

- **Access:**  
  - `/staff` — Staff dashboard  
  - `/serve` — Serve orders  
  - `/cashier` — Cashier/payment management  
  - `/order-history` — View all order history

- **Features:**  
  - Real-time order updates  
  - See what needs to be served  
  - Mark orders as served  
  - Manage payments at cashier  
  - View complete order history

---

## Customer Ordering

- **Features:**  
  - Browse food categories and menus  
  - Add items to cart  
  - Place orders for your table  
  - View your order history and payment status

---

## Payment Flow

- **QR Code Payment:**  
  - On the payment page, choose "QR Code PromptPay".
  - Scan the generated QR code with your mobile device.  
  - _(For demo: use the skip button instead of scanning QR code)_
  - The payment page will automatically redirect or close when payment is confirmed.

- **Cashier Payment:**  
  - Choose "Pay at Cashier" on the payment page.
  - Go to the cashier desk to complete your payment.
  - Staff can mark your payment as complete from the staff panel.

---

## Real-Time Features

- All order and payment updates are pushed instantly to staff and customer screens using Socket.io.
- Staff and customers see live status changes without refreshing.

---

## Developer Notes

- **Demo Mode:**  
  If `table_id` is missing, the app will auto-assign `0` and update the URL.
- **Customization:**  
  You can change food categories, menu items, and images in the `/categories` folder.

---

**Enjoy your demo! If you have questions or want to contribute, open an issue or pull request.**
