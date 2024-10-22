- 👋 Hi, I’m @Nudelssssss
- 👀 I’m interested in ...
- 🌱 I’m currently learning ...
- 💞️ I’m looking to collaborate on ...
- 📫 How to reach me ...
- 😄 Pronouns: ...
- ⚡ Fun fact: ...

<!---
Nudelssssss/Nudelssssss is a ✨ special ✨ repository because its `README.md` (this file) appears on your GitHub profile.
You can click the Preview link to take a look at your changes.
--->

<!DOCTYPE html>
<html>
<head>
 <title>Coffee Shop</title>
</head>
<body>
 <h1>Coffee Shop</h1>
 <ul id="menu">
 <li>Coffee</li>
 <li>Tea</li>
 <li>Smoothie</li>
 </ul>
 <form id="order-form">
 <label>Name:</label>
 <input type="text" id="name" />
 <label>Order:</label>
 <select id="order">
 <option>Coffee</option>
 <option>Tea</option>
 <option>Smoothie</option>
 </select>
 <label>Quantity:</label>
 <input type="number" id="quantity" />
 <button id="order-btn">Order</button>
 </form>
 <div id="payment-gateway">
 <!-- Integrate payment gateway here -->
 </div>
 <script src="script.js"></script>
</body>
</html>
```

CSS:
```
body {
 font-family: Arial, sans-serif;
}

#menu {
 list-style: none;
 padding: 0;
 margin: 0;
}

#order-form {
 margin-top: 20px;
}

#order-form label {
 display: block;
 margin-bottom: 10px;
}

#order-form input, #order-form select {
 width: 100%;
 height: 30px;
 margin-bottom: 20px;
 padding: 10px;
 box-sizing: border-box;
}

#order-btn {
 background-color: #4CAF50;
 color: #fff;
 padding: 10px 20px;
 border: none;
 border-radius: 5px;
 cursor: pointer;
}

#order-btn:hover {
 background-color: #3e8e41;
}
```

JavaScript (sa script.js file):
```
const orderForm = document.getElementById('order-form');
const orderBtn = document.getElementById('order-btn');

orderBtn.addEventListener('click', (e) => {
 e.preventDefault();
 const name = document.getElementById('name').value;
 const order = document.getElementById('order').value;
 const quantity = document.getElementById('quantity').value;
 
 // Send order data to server or payment gateway
 console.log(`Order: ${name} - ${order} x ${quantity}`);
});
```
