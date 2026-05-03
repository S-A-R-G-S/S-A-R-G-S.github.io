[index.html.html](https://github.com/user-attachments/files/27311545/index.html.html)
<!DOCTYPE html>
<html lang="es">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <title>J.J Components | Electrónica y mas</title>
  <style>
    body {
      font-family: Arial, sans-serif;
      margin: 0;
      padding: 0;
      background-color: #f4f4f4;
      color: #333;
    }
  
    header {
      background-color: #1e3a8a;
      color: white;
      padding: 15px 0;
      text-align: center;
    }
  
    .logo {
      font-size: 2.5rem;
      font-weight: bold;
    }
  
    nav {
      background-color: #1e40af;
      padding: 12px;
      text-align: center;
      display: flex;
      flex-wrap: wrap;
      justify-content: center;
      align-items: center;
      gap: 15px;
    }
  
    nav a {
      color: white;
      text-decoration: none;
      font-size: 1.1rem;
    }

    /* Barra de búsqueda */
    .search-container {
      display: flex;
      align-items: center;
      background: white;
      border-radius: 25px;
      padding: 5px 10px;
      max-width: 350px;
      width: 100%;
    }

    .search-container input {
      border: none;
      outline: none;
      padding: 8px 12px;
      width: 100%;
      font-size: 1rem;
    }

    .search-container button {
      background-color: #1e40af;
      color: white;
      border: none;
      padding: 8px 16px;
      border-radius: 20px;
      cursor: pointer;
      font-size: 1rem;
    }

    .hero {
      background-color: #1e40af;
      color: white;
      text-align: center;
      padding: 60px 20px;
    }
    .section {
      padding: 40px 20px;
      text-align: center;
    }
    .cards {
      display: flex;
      flex-wrap: wrap;
      justify-content: center;
      gap: 20px;
      margin-top: 20px;
    }
  
    .card {
      background: white;
      border: 1px solid #ddd;
      border-radius: 10px;
      width: 280px;
      overflow: hidden;
      box-shadow: 0 4px 8px rgba(0,0,0,0.1);
    }
  
    .card img {
      width: 100%;
      height: 180px;
      object-fit: cover;
    }
  
    .card h3 {
      margin: 10px 0 5px;
    }
  
    .btn-comprar {
      background-color: #1e40af;
      color: white;
      padding: 10px 20px;
      border: none;
      border-radius: 5px;
      cursor: pointer;
      margin: 10px 0;
    }
    .modal {
      display: none;
      position: fixed;
      top: 0; left: 0;
      width: 100%; height: 100%;
      background: rgba(0,0,0,0.7);
      z-index: 1000;
    }
  
    .modal-content {
      background: white;
      margin: 5% auto;
      padding: 20px;
      width: 90%;
      max-width: 400px;
      border-radius: 10px;
      text-align: center;
    }
    form {
      max-width: 500px;
      margin: 0 auto;
      background: white;
      padding: 25px;
      border-radius: 10px;
      box-shadow: 0 4px 8px rgba(0,0,0,0.1);
    }
  
    input {
      width: 100%;
      padding: 10px;
      margin: 10px 0;
      border: 1px solid #ccc;
      border-radius: 5px;
    }
  
    button {
      background-color: #1e40af;
      color: white;
      padding: 12px 25px;
      border: none;
      border-radius: 5px;
      font-size: 1.1rem;
      cursor: pointer;
      width: 100%;
    }
    .redes-sociales {
      margin-top: 25px;
    }
   
    .redes-sociales a {
      color: #1e40af;
      font-size: 1.5rem;
      margin: 0 12px;
      text-decoration: none;
    }

    /* Pie de página mejorado */
    footer {
      background-color: #1e3a8a;
      color: white;
      text-align: center;
      padding: 40px 20px;
      margin-top: 50px;
    }

    .footer-content {
      max-width: 1000px;
      margin: 0 auto;
    }

    .footer-links {
      display: flex;
      flex-wrap: wrap;
      justify-content: center;
      gap: 20px;
      margin: 20px 0;
    }

    .footer-links a {
      color: white;
      text-decoration: none;
    }
  </style>
</head>
<body>
  <header>
    <div class="logo">J.J Components</div>
  </header>

  <nav>
    <a href="#inicio">Inicio</a>
    <a href="#productos">Productos</a>
    <a href="#cuenta">Crear Cuenta</a>
    <a href="#contacto">Contacto</a>

    <!-- Barra de búsqueda -->
    <form id="searchForm" class="search-container">
      <input type="text" id="searchInput" placeholder="Buscar productos...">
      <img src="https://img.icons8.com/?size=160&id=e4NkZ7kWAD7f&format=png" alt="Buscar" style="width: 20px; height: 20px;">
      <button type="submit">Buscar</button>
    </form>
  </nav>

  <section id="inicio" class="hero">
    <h1>Bienvenidos a J.JComponents</h1>
    <p>Tu tienda de electrónica en Panamá</p>
  </section>

  <!-- PRODUCTOS -->
  <section id="productos" class="section" style="background:white;">
    <h2>Productos Destacados</h2>
  
    <div class="cards">
      <div class="card">
        <img src="https://m.media-amazon.com/images/I/51Ci8gnvlAL._AC_SX466_.jpg" alt="Arduino">
        <div style="padding:15px;">
          <h3>Arduino Uno</h3>
          <p><strong>$24.99</strong></p>
          <button class="btn-comprar" onclick="comprar('Arduino Uno', 24.99)">Comprar</button>
        </div>
      </div>
    
      <div class="card">
        <img src="https://m.media-amazon.com/images/I/71HeXwnzjbL._AC_SX679_.jpg" alt="LED">
        <div style="padding:15px;">
          <h3>Tira LED RGB 5m</h3>
          <p><strong>$14.99</strong></p>
          <button class="btn-comprar" onclick="comprar('Tira LED RGB', 14.99)">Comprar</button>
        </div>
      </div>
    
      <div class="card">
        <img src="https://m.media-amazon.com/images/I/81hR7vU0xQL._AC_SY879_.jpg" alt="Kit">
        <div style="padding:15px;">
          <h3>Kit Básico Electrónica</h3>
          <p><strong>$39.99</strong></p>
          <button class="btn-comprar" onclick="comprar('Kit Básico Electrónica', 39.99)">Comprar</button>
        </div>
      </div>
    </div>
  </section>

  <!-- VIDEO -->
  <section class="section">
    <h2>Video Recomendado</h2>
    <iframe width="360" height="640"
      src="https://www.youtube.com/embed/q-jeD6gANcQ"
      title="YouTube video player"
      frameborder="0"
      allowfullscreen>
    </iframe>
  </section>

  <!-- CONTACTO -->
  <section id="contacto" class="section">
    <h2>Contáctanos</h2>
    <p>WhatsApp: <strong>+507 6000-0000</strong></p>
   
    <div class="redes-sociales">
      <h3>Síguenos en redes:</h3>
      <a href="https://instagram.com/jjcomponents" target="_blank"><img src="https://pbs.twimg.com/profile_images/730398192169328640/aN0B-LIm_400x400.jpg" alt="Instagram" style="width: 30px; height: 30px; margin-right: 10px;"> Instagram: @jjcomponents</a><br><br>
      <a href="https://x.com/jjcomponents" target="_blank"><img src="https://1000marcas.net/wp-content/uploads/2025/04/X-Logo.png" alt="X (Twitter)" style="width: 30px; height: 30px; margin-right: 10px;"> X (Twitter): @jjcomponents</a>
    </div>
  </section>

  <!-- MODAL DE COMPRA -->
  <div id="modalCompra" class="modal">
    <div class="modal-content">
      <h3>¡Producto agregado al carrito!</h3>
      <p id="modalProducto"></p>
      <p><strong>Precio: $<span id="modalPrecio"></span></strong></p>
      <button onclick="cerrarModal()" style="background:#333; margin-top:15px;">Cerrar</button>
    </div>
  </div>

  <!-- PIE DE PÁGINA (FOOTER) MEJORADO -->
  <footer>
    <div class="footer-content">
      <p><strong>J.J Components © 2026</strong> - Todos los derechos reservados</p>
      <p>Panamá | Tienda de Componentes Electrónicos</p>
      
      <div class="footer-links">
        <a href="#inicio">Inicio</a>
        <a href="#productos">Productos</a>
        <a href="#contacto">Contacto</a>
        <a href="#">Política de Privacidad</a>
        <a href="#">Términos de Servicio</a>
      </div>
      
    </div>
  </footer>

  <script>
    // Función de búsqueda
    document.getElementById('searchForm').addEventListener('submit', function(e) {
      e.preventDefault();
      const searchTerm = document.getElementById('searchInput').value.trim();
      
      if (searchTerm === "") {
        alert("Por favor ingresa un término de búsqueda.");
        return;
      }
      
      alert("De momento la barra de búsqueda no funciona.\n\nEstamos trabajando para mejorar esta función.");
      // Redirigir al inicio
      window.location.href = "#inicio";
      
      // Opcional: limpiar el campo
      document.getElementById('searchInput').value = "";
    });

    function comprar(producto, precio) {
      document.getElementById("modalProducto").textContent = producto;
      document.getElementById("modalPrecio").textContent = precio;
      document.getElementById("modalCompra").style.display = "block";
    }
  
    function cerrarModal() {
      document.getElementById("modalCompra").style.display = "none";
    }
  
    function crearCuenta(event) {
      event.preventDefault();
      alert(" ¡Cuenta creada exitosamente! (Esto es solo una simulación)");
    }
  </script>
</body>
</html>
