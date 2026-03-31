<!DOCTYPE html>
<html>
<head>
  <Xscar7D>Store Me</Don>

  <style>
    body {
      font-family: Arial;
      background: #111;
      color: white;
      text-align: center;
    }

    h1 {
      color: #00ffcc;
    }

    .product {
      border: 1px solid #444;
      padding: 20px;
      margin: 20px;
      border-radius: 10px;
      background: #222;
    }

    img {
      width: 150px;
    }

    button {
      background: green;
      color: white;
      padding: 10px;
      border: none;
      cursor: pointer;
      border-radius: 5px;
    }

    button:hover {
      background: darkgreen;
    }

    #cart {
      margin-top: 20px;
      font-size: 18px;
    }
  </style>
</head>

<body>

<h1>🛒 Store Mwen</h1>

<div class="product">
  <img src="https://via.placeholder.com/150">
  <h2>Soulye Nike</h2>
  <p>Prix: $50</p>
  <button onclick="achte(50)">Achte</button>
</div>

<div class="product">
  <img src="https://via.placeholder.com/150">
  <h2>Telefòn Samsung</h2>
  <p>Prix: $120</p>
  <button onclick="achte(120)">Achte</button>
</div>

<div id="cart">
  🛒 Total: $0
</div>

<script>
let total = 0;

function achte(prix) {
  total += prix;
  document.getElementById("cart").innerText = "🛒 Total: $" + total;
}
</script>

</body>
</html>
