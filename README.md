# Campus-Bazaar: Pre-Loved Textbook & Gear Exchange

**Course:** CSC584 — Enterprise Programming  
**Faculty:** Faculty of Computer and Mathematical Sciences, Universiti Teknologi MARA (UiTM)
**Group:** Group 1 
**Lecturer:** Muhamad Ridhwan Bin Mohamad Razali
**Proposal Document:** `CSC584 Project Proposal (2025126993).pdf

---

## 1.0 Introduction

**Campus-Bazaar** is a digital marketplace designed for university students to buy, sell, and exchange used textbooks and other campus items[cite: 7]. Students can list pre-loved items, search and filter listings by keywords, prices, and faculty categories, and submit purchase requests. Sellers can update item availability, administrators can remove inappropriate listings, and a dashboard highlights popular item categories, total exchange value, and active user growth

---

## 2.0 Objectives

1. Develop an online platform for students to buy, sell, and exchange used textbooks and campus items
2. Enable students to create, view, and update item listings and submit purchase requests

---

## 3.0 System Workflows (Flowcharts)

- **Main System Flow:** Users access the platform, view the homepage, select a role (**Seller**, **Buyer**, or **Admin**), complete role-specific tasks, and log out[cite: 9, 10].
- **Buyer Flow:** Log in as a buyer, view listings, filter by keyword/price range/faculty category, inspect item details, and create/save a purchase request[cite: 11, 12].
- **Admin Flow:** Log in to the admin panel, review flagged posts, decide whether to keep or delete reported listings, and finish[cite: 13, 14].
- **Seller Flow:** Log in as a seller, enter item details (name, description, price, category, condition, availability), validate and save/publish the listing, and optionally update status (`Sold` / `Unavailable`)[cite: 14, 15].

---

## 4.0 Database Design (ERD Overview)

Core entities in the proposal ERD[cite: 16]:

- `USER` (`User_ID`, `FullName`, `Email`, `Password`, `PhoneNumber`, `Role`, `Faculty`, `RegistrationDate`)
- `CATEGORY` (`Category_ID`, `CategoryName`, `CategoryDescription`)
- `ITEM LISTING` (`Item_ID`, `UserID`, `CategoryID`, `Name`, `Description`, `Price`, `Condition`, `Image`, `AvailabilityStatus`, `PostingDate`)
- `PURCHASE REQUEST` (`Request_ID`, `UserID`, `ItemID`, `RequestDate`, `RequestStatus`, `Quantity`)
- `TRANSACTION` (`Transaction_ID`, `RequestID`, `TransactionDate`, `TotalAmount`, `TransactionStatus`)
- `FLAGGED POST` (`Flag_ID`, `ItemID`, `UserID`, `Reason`, `ReportDate`, `FlagStatus`)
- `ADMIN_ACTION` (`Action_ID`, `UserID`, `FlagID`, `ActionType`, `ActionDate`)

---

## 5.0 Storyboard Screens

1. **Main / Home Page:** Promotional banners, featured/new arrivals, and navigation across the store flow[cite: 17].
2. **Product List Page:** Browse items with category/size/price/sale filters and sorting[cite: 18].
3. **Product Details Page:** View item pricing, size/variant options, description, material details, and quantity before adding to cart[cite: 19].
4. **Shopping Cart Page:** Adjust item quantities, remove items, and review subtotal, shipping, and total before checkout[cite: 20].
5. **Checkout Page:** Enter shipping details, choose delivery option, pick a payment method, and place the order[cite: 21].
6. **Order Confirmation Page:** Displays order confirmation details and status after checkout.

---

