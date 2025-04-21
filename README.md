<!DOCTYPE html>
<html lang="es">
<head>
  <meta charset="UTF-8" />
  <meta name="viewport" content="width=device-width, initial-scale=1.0"/>
  <title>Delicias Dulces</title>
  <style>
    body {
      font-family: 'Segoe UI', sans-serif;
      background-color: #fff8f0;
      margin: 0;
      padding: 0;
    }

    header {
      background-color: #ff6f61;
      color: white;
      padding: 20px;
      text-align: center;
    }

    h2 {
      text-align: center;
      color: #ff6f61;
      margin-top: 40px;
    }

    .container {
      display: grid;
      grid-template-columns: repeat(auto-fit, minmax(250px, 1fr));
      gap: 20px;
      padding: 40px;
    }

    .card {
      background-color: #fff;
      border-radius: 15px;
      box-shadow: 0 4px 8px rgba(0,0,0,0.1);
      overflow: hidden;
      transition: transform 0.3s;
    }

    .card:hover {
      transform: scale(1.03);
    }

    .card img {
      width: 100%;
      height: 200px;
      object-fit: cover;
    }

    .card-content {
      padding: 15px;
    }

    .card-title {
      font-size: 1.2em;
      margin-bottom: 10px;
    }

    .card-description {
      font-size: 0.95em;
      color: #555;
      margin-bottom: 15px;
    }

    .buy-button {
      background-color: #ff6f61;
      color: white;
      padding: 10px 15px;
      border: none;
      border-radius: 8px;
      cursor: pointer;
      text-decoration: none;
      font-weight: bold;
    }

    .buy-button:hover {
      background-color: #e4574f;
    }

    footer {
      text-align: center;
      padding: 20px;
      background-color: #ffe5dc;
      color: #333;
    }
  </style>
</head>
<body>
  <header>
    <h1>Delicias Dulces</h1>
    <p>¡Endulza tu día con nuestros postres caseros!</p>
  </header>

  <!-- POSTRES -->
  <h2>Postres</h2>
  <div class="container">
    <!-- 10 postres en total -->
    <div class="card">
      <img src="data:image/jpeg;base64,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" alt="Cheesecake">
      <div class="card-content">
        <h3 class="card-title">Cheesecake de Frutilla</h3>
        <p class="card-description">Cremoso con base crocante y frutillas frescas.</p>
           <p>$8.000</p>
        <a href="#" class="buy-button">Comprar</a>
      </div>
    </div>

    <div class="card">
      <img src="https://cdn.recetasderechupete.com/wp-content/uploads/2019/11/Brownie.jpg" alt="Brownies">
      <div class="card-content">
        <h3 class="card-title">Brownies Clásicos</h3>
        <p class="card-description">Brownies de chocolate con centro fundente.</p>
   <p>$5.000</p>
        <a href="#" class="buy-button">Comprar</a>
      </div>
    </div>

    <div class="card">
      <img src="https://encrypted-tbn0.gstatic.com/images?q=tbn:ANd9GcQ0qJaE1ud1bb6ZrwKMVnbZ2nTxvBZn8Kv9zw&s" alt="Cupcakes">
      <div class="card-content">
        <h3 class="card-title">Cupcakes Variados</h3>
        <p class="card-description">Pack de vainilla, chocolate y red velvet.</p>
           <p>$4.000</p>
        <a href="#" class="buy-button">Comprar</a>
      </div>
    </div>

    <div class="card">
      <img src="https://encrypted-tbn0.gstatic.com/images?q=tbn:ANd9GcQpuOWD3FgG4EyHWunhPN2wk3M3aJlNB7xDIA&s" alt="Tarta de Manzana">
      <div class="card-content">
        <h3 class="card-title">Tarta de Manzana</h3>
        <p class="card-description">Manzanas caramelizadas y toque de canela.</p>
           <p>$22.000</p>
        <a href="#" class="buy-button">Comprar</a>
      </div>
    </div>

    <div class="card">
      <img src="https://encrypted-tbn0.gstatic.com/images?q=tbn:ANd9GcR-wxQ8IM1bsBGGy9RKkjFW1K47Urqk55Mkfg&s" alt="Tiramisú">
      <div class="card-content">
        <h3 class="card-title">Tiramisú Italiano</h3>
        <p class="card-description">Clásico con café, mascarpone y cacao.</p>
            <p>$9.000</p>
        <a href="#" class="buy-button">Comprar</a>
      </div>
    </div>

    <div class="card">
      <img src="https://i.ytimg.com/vi/a1tDpcCDCyo/maxresdefault.jpg" alt="Macarons">
      <div class="card-content">
        <h3 class="card-title">Macarons Franceses</h3>
        <p class="card-description">Coloridos, crocantes y suaves por dentro.</p>
            <p>$2.000</p>
        <a href="#" class="buy-button">Comprar</a>
      </div>
    </div>

    <div class="card">
      <img src="https://encrypted-tbn0.gstatic.com/images?q=tbn:ANd9GcTvhH3GdfVPOznOxJkk61-6DYKZiSnZuo8lIw&s" alt="Tarta de limón">
      <div class="card-content">
        <h3 class="card-title">Tarta de Limón</h3>
        <p class="card-description">Refrescante crema de limón con merengue.</p>
           <p>$22.000</p>
        <a href="#" class="buy-button">Comprar</a>
      </div>
    </div>

    <div class="card">
      <img src="https://encrypted-tbn0.gstatic.com/images?q=tbn:ANd9GcTomlOcmV0NtC8Ov-EniuGbcycjET1OqW2oww&s" alt="Profiteroles">
      <div class="card-content">
        <h3 class="card-title">Profiteroles</h3>
        <p class="card-description">Rellenos de crema pastelera y bañados en chocolate.</p>
   <p>$1.500</p>
        <a href="#" class="buy-button">Comprar</a>
      </div>
    </div>

    <div class="card">
      <img src="https://encrypted-tbn0.gstatic.com/images?q=tbn:ANd9GcQQmnS53eaA5Uqlz4NOmtx3lD_wCJ1L7T8SKA&s" alt="Alfajores">
      <div class="card-content">
        <h3 class="card-title">Alfajores Artesanales</h3>
        <p class="card-description">De maicena, con dulce de leche y coco.</p>
            <p>$3.000</p>
        <a href="#" class="buy-button">Comprar</a>
      </div>
    </div>

    <div class="card">
      <img src="https://sabrosano.com/wp-content/uploads/2020/05/Donas-Glaseadas-Paso-4.jpg" alt="Donas">
      <div class="card-content">
        <h3 class="card-title">Donas Glaseadas</h3>
        <p class="card-description">Suaves, dulces y con coberturas de colores.</p>
           <p>$6.000</p>
        <a href="#" class="buy-button">Comprar</a>
      </div>
    </div>
  </div>

  <!-- BEBIDAS -->
  <h2>Bebidas</h2>
  <div class="container">
    <div class="card">
      <img src="https://encrypted-tbn0.gstatic.com/images?q=tbn:ANd9GcRjwLvUuzAtUoTL4VtROCKn2zIyDOwXqCwRxQ&s" alt="Café">
      <div class="card-content">
        <h3 class="card-title">Café Espresso</h3>
        <p class="card-description">Café intenso, ideal para acompañar postres.</p>
           <p>$5.000</p>
        <a href="#" class="buy-button">Comprar</a>
      </div>
    </div>

    <div class="card">
      <img src="https://encrypted-tbn0.gstatic.com/images?q=tbn:ANd9GcQNmaFVa0lGGq3Ay8gz-yq4lrG0VTIdgx0CMQ&s" alt="Té">
      <div class="card-content">
        <h3 class="card-title">Té Artesanal</h3>
        <p class="card-description">Tés seleccionados de frutas y hierbas.</p>
        <a href="#" class="buy-button">Comprar</a>
           <p>$4.000</p>
      </div>
    </div>

    <div class="card">
      <img src="https://img-global.cpcdn.com/recipes/ee6ccbd8fd213190/400x400cq70/photo.jpg" alt="Chocolate caliente">
      <div class="card-content">
        <h3 class="card-title">Chocolate Caliente</h3>
        <p class="card-description">Espeso, cremoso y con mini malvaviscos.</p>
            <p>$7.000</p>
        <a href="#" class="buy-button">Comprar</a>
      </div>
    </div>

    <div class="card">
      <img src="https://encrypted-tbn0.gstatic.com/images?q=tbn:ANd9GcT6EOPLU9mtiSCE9FqKSY67iA8qep_-muf80g&s" alt="Limonada">
      <div class="card-content">
        <h3 class="card-title">Limonada Natural</h3>
        <p class="card-description">Refrescante, con limón y menta fresca.</p>
            <p>$9.000</p>
        <a href="#" class="buy-button">Comprar</a>
      </div>
    </div>
  </div>

  <footer>
    <p>&copy; 2025 Delicias Dulces - Todos los derechos reservados</p>
  </footer>
</body>
</html>
