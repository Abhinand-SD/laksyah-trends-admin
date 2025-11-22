🛠️ Admin Panel — Features & Overview

This Admin Panel is part of my MERN Stack E-commerce application. It provides complete control over users, categories, and products, along with advanced UI interactions such as size selection, bestseller toggle, and more.

🚀 Admin Features
✅ 1. Admin Authentication

Secure admin sign-in

JWT-based authentication

Protects all admin routes

👥 2. User Management

View all users

Block / Unblock users

Delete users

Search users

🗂️ 3. Category Management

Add new categories

Edit categories

Soft delete categories

Validation for duplicate names

📦 4. Product Management

Add new products

Edit product details

Delete / Soft delete products

Upload multiple images (min. 3 images)

Image cropping & resizing before upload

Manage:

Ratings

Price

Stock

Highlights/specs

Discounts / Coupons

Related product recommendations

🎚️ 5. Product Size Selector

Example code used in product form:

<div onClick={() =>
  setSizes(prev =>
    prev.includes("L")
      ? prev.filter(item => item !== "L")
      : [...prev, "L"]
  )
}>
  <p className="bg-slate-200 px-3 py-1 cursor-pointer">L</p>
</div>


✔ Adds/removes sizes dynamically
✔ Fully controlled React state

⭐ 6. Bestseller Toggle

Uses a controlled checkbox:

<input
  type="checkbox"
  id="bestseller"
  checked={bestseller}
  onChange={() => setBestseller(prev => !prev)}
/>
<label htmlFor="bestseller">Add to Bestseller</label>


✔ Uses checked={bestseller} (required for controlled input)
✔ Clean onChange handler

🧰 Tech Stack

Frontend: React.js, Tailwind CSS

Backend: Node.js, Express.js

Database: MongoDB

Auth: JWT

File Upload: Multer, Sharp (for cropping/resizing)

📌 How to Run
Clone Repository
git clone https://github.com/yourusername/yourrepo.git

Install Dependencies
npm install

Start Server
npm start


If you want, I can also:

✅ Add screenshots
✅ Add deployment link
✅ Format this for full project README
✅ Create separate sections for backend & frontend
