# kahmoh6.github.io
clothing-boutique/
│── backend/              # Node.js + Express API
│   ├── models/           # Product, User, Order schemas
│   ├── routes/           # API endpoints
│   ├── controllers/      # Logic for products/cart/orders
│   ├── server.js         # Main server file
│── frontend/             # React + Tailwind frontend
│   ├── src/
│   │   ├── pages/        # Home, Shop, Product, Cart, Checkout
│   │   ├── components/   # Navbar, Footer, ProductCard, etc.
│   │   ├── context/      # Cart + Auth state
│   │   └── App.js
│── package.json
// src/pages/Home.js
import { useEffect, useState } from "react";
import ProductCard from "../components/ProductCard";

export default function Home() {
  const [products, setProducts] = useState([]);

  useEffect(() => {
    fetch("http://localhost:5000/api/products")
      .then(res => res.json())
      .then(data => setProducts(data));
  }, []);

  return (
    <div className="p-8">
      <h1 className="text-4xl font-bold mb-6">Welcome to Luxe Boutique</h1>
      <div className="grid grid-cols-1 sm:grid-cols-2 md:grid-cols-3 gap-6">
        {products.map(p => (
          <ProductCard key={p._id} product={p} />
        ))}
      </div>
      // src/pages/Home.js
import { useEffect, useState } from "react";
import ProductCard from "../components/ProductCard";

export default function Home() {
  const [products, setProducts] = useState([]);

  useEffect(() => {
    fetch("http://localhost:5000/api/products")
      .then(res => res.json())
      .then(data => setProducts(data));
  }, []);

  return (
    <div className="p-8">
      <h1 className="text-4xl font-bold mb-6">Welcome to Luxe Boutique</h1>
      <div className="grid grid-cols-1 sm:grid-cols-2 md:grid-cols-3 gap-6">
        {products.map(p => (
          <ProductCard key={p._id} product={p} />
        ))}
      </div>
    </div>
  );
}
// backend/routes/productRoutes.js
import express from "express";
import Product from "../models/Product.js";

const router = express.Router();

// Get all products
router.get("/", async (req, res) => {
  const products = await Product.find();
  res.json(products);
});

// Add a product
router.post("/", async (req, res) => {
  const newProduct = new Product(req.body);
  await newProduct.save();
  res.json(newProduct);
});

export default router;

    </div>
  );
}
