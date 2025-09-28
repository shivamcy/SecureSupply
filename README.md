# Decentralized Supply Chain & Order Tracking System

A **decentralized supply chain management system** that allows **buyers, sellers, middlemen, and delivery admins** to track orders transparently using **Web3 and IPFS**, ensuring tamper-proof, verifiable delivery records.

---

## 🔹 Features

### User Management
- **Signup & Login** with JWT authentication.
- **Role-based access:** Buyer, Seller, Middleman, Delivery Admin.
- **Profile Management:** Users can view their profile.

### Product Management
- **Add Products:** Sellers can add products with images.
- **View Products:** Buyers can browse all products; sellers can view their own.

### Order Management
- **Place Orders:** Buyers can place orders for available products.
- **Track Orders:** Delivery admins can manage order tracks including sellers, middlemen, and buyers.
- **Order Queue Management:** Delivery admins manage pending orders efficiently.
- **Transaction Verification:** Current owner verifies order transfer using OTP.

### Web3 & IPFS Integration
- **Decentralized Storage:** Order tracks are uploaded to IPFS using **Pinata SDK**.
- **Blockchain Reference:** Web3 integration ensures track immutability and transparency.
- **Download Tracks:** Users can fetch order history directly from IPFS.

### Security
- **OTP-secured Transfers:** Adds a layer of authentication for each delivery step.
- **Role-based Permissions:** Only authorized users can perform specific actions.
- **Immutable Tracking:** Prevents tampering using IPFS and Web3.

---

## 🔹 Tech Stack

- **Frontend:** React.js (for dashboards and UI)
- **Backend:** Node.js + Express.js
- **Database:** MongoDB (Mongoose)
- **Authentication:** JWT, bcrypt
- **File Uploads:** Multer, Cloudinary
- **Decentralized Storage:** IPFS (via Pinata SDK)
- **Blockchain Interaction:** Web3.js
- **Logging:** Winston or custom logger
- **Other:** Async handling, structured API responses

---

## 🔹 System Flow

1. **User Registration & Login**
2. **Product Management**
   - Sellers add products
   - Buyers browse products
3. **Order Creation**
   - Buyers place orders
   - Delivery Admin receives orders in queue
4. **Order Tracking**
   - Delivery Admin adds track with seller, buyer, and middlemen
   - Track uploaded to IPFS
5. **Transaction Verification**
   - OTP generated and verified for ownership transfer
   - Statuses updated and reflected in Web3
6. **Order Completion**
   - Order marked as delivered
   - Entries removed from users and database

---


