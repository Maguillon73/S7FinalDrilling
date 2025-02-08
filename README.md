<!DOCTYPE html>
<html lang="es">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Portafolio Profesional - Maximiliano Aguillón</title>
    <link rel="stylesheet" href="styles.css">
    <style>
        body {
            font-family: 'Arial', sans-serif;
            margin: 0;
            padding: 0;
            background: #f7f7f7;
            color: #333;
        }
        header {
            background: #1e3a5f;
            color: white;
            padding: 30px 0;
            text-align: center;
        }
        header h1 {
            font-size: 2.5em;
        }
        nav ul {
            list-style: none;
            padding: 0;
            margin-top: 20px;
        }
        nav ul li {
            display: inline-block;
            margin: 0 15px;
        }
        nav ul li a {
            color: white;
            text-decoration: none;
            font-weight: bold;
            text-transform: uppercase;
            letter-spacing: 1px;
        }
        section {
            margin: 50px auto;
            width: 80%;
            padding: 30px;
            background: white;
            border-radius: 10px;
            box-shadow: 0 5px 15px rgba(0, 0, 0, 0.1);
        }
        h2 {
            font-size: 2em;
            color: #1e3a5f;
            margin-bottom: 20px;
        }
        .proyectos, .testimonios {
            display: grid;
            grid-template-columns: repeat(3, 1fr);
            gap: 20px;
        }
        .proyecto, .testimonio {
            background: #fff;
            border-radius: 10px;
            padding: 20px;
            box-shadow: 0px 0px 10px rgba(0, 0, 0, 0.05);
            transition: transform 0.3s ease, box-shadow 0.3s ease;
        }
        .proyecto:hover, .testimonio:hover {
            transform: translateY(-10px);
            box-shadow: 0px 10px 20px rgba(0, 0, 0, 0.1);
        }
        .proyecto img, .testimonio img {
            width: 100%;
            height: auto;
            border-radius: 10px;
        }
        .proyecto h3 {
            color: #1e3a5f;
            font-size: 1.5em;
            margin-top: 15px;
        }
        .proyecto p {
            color: #555;
        }
        .testimonio p {
            font-style: italic;
            color: #666;
            margin-top: 10px;
        }
        .nombre {
            font-weight: bold;
            margin-top: 5px;
        }
        .testimonio .avatar {
            border-radius: 50%;
            width: 60px;
            height: 60px;
            overflow: hidden;
            margin-right: 15px;
        }
        .testimonio .avatar img {
            width: 100%;
            height: 100%;
            object-fit: cover;
        }
        .testimonio .contenedor-testimonio {
            display: flex;
            align-items: center;
        }
        button {
            background: #28a745;
            color: white;
            padding: 10px 20px;
            border: none;
            cursor: pointer;
            border-radius: 5px;
            transition: background-color 0.3s;
        }
        button:hover {
            background-color: #218838;
        }
        form {
            display: flex;
            flex-direction: column;
            gap: 15px;
        }
        form label {
            font-size: 1.1em;
            margin-bottom: 5px;
        }
        form input, form textarea {
            padding: 10px;
            font-size: 1em;
            border: 1px solid #ccc;
            border-radius: 5px;
        }
        form textarea {
            height: 150px;
            resize: vertical;
        }
        .carrito {
            background: #fff;
            padding: 20px;
            border-radius: 10px;
            box-shadow: 0px 0px 10px rgba(0, 0, 0, 0.1);
        }
        .producto-carrito {
            display: flex;
            justify-content: space-between;
            padding: 15px 0;
            border-bottom: 1px solid #eee;
        }
        .producto-carrito p {
            margin: 0;
        }
        .estrellas {
            color: #f1c40f;
            font-size: 20px;
        }
        .comentarios {
            margin-top: 20px;
        }
        .comentarios textarea {
            width: 100%;
            height: 80px;
            padding: 10px;
            margin-top: 10px;
        }
        .comentarios button {
            background: #3498db;
        }
        @media (max-width: 1024px) {
            .proyectos, .testimonios {
                grid-template-columns: repeat(2, 1fr);
            }
        }
        @media (max-width: 768px) {
            .proyectos, .testimonios {
                grid-template-columns: 1fr;
            }
        }
    </style>
</head>
<body>
    <header>
        <h1>Portafolio Profesional de Maximiliano Aguillón</h1>
        <nav>
            <ul>
                <li><a href="#sobre-mi">Sobre Mí</a></li>
                <li><a href="#proyectos">Proyectos</a></li>
                <li><a href="#testimonios">Testimonios</a></li>
                <li><a href="#carrito">Carrito de Compras</a></li>
                <li><a href="#contacto">Contacto</a></li>
            </ul>
        </nav>
    </header>

    <section id="sobre-mi">
        <h2>Sobre Mí</h2>
        <p>Soy Maximiliano Aguillón, un analista programador con experiencia en backend, frontend, Java, CSS y más. Apasionado por el desarrollo web y la optimización de procesos tecnológicos.</p>
    </section>

    <section id="proyectos">
        <h2>Proyectos</h2>
        <div class="proyectos">
            <div class="proyecto">
                <img src="https://via.placeholder.com/400x200" alt="Proyecto 1">
                <h3>Proyecto 1 - Gestión de Inventarios</h3>
                <p>Un sistema de gestión de inventarios desarrollado en Java y MySQL, diseñado para optimizar el control de productos en almacenes.</p>
                <button onclick="agregarAlCarrito('Proyecto 1', 1000)">Agregar al carrito</button>
            </div>
            <div class="proyecto">
                <img src="https://via.placeholder.com/400x200" alt="Proyecto 2">
                <h3>Proyecto 2 - Tienda en Línea</h3>
                <p>Un sitio web responsivo con carrito de compras y pago en línea, utilizando tecnologías como HTML, CSS, JavaScript y PHP.</p>
                <button onclick="agregarAlCarrito('Proyecto 2', 500)">Agregar al carrito</button>
            </div>
            <div class="proyecto">
                <img src="https://via.placeholder.com/400x200" alt="Proyecto 3">
                <h3>Proyecto 3 - Dashboard de Análisis</h3>
                <p>Un dashboard interactivo en Power BI para la visualización y análisis de datos empresariales en tiempo real.</p>
                <button onclick="agregarAlCarrito('Proyecto 3', 300)">Agregar al carrito</button>
            </div>
        </div>
    </section>

    <section id="carrito">
        <h2>Carrito de Compras</h2>
        <div class="carrito" id="carrito-container">
            <p>No hay productos en tu carrito.</p>
        </div>
    </section>

    <section id="testimonios">
        <h2>Testimonios</h2>
        <div class="testimonios">
            <div class="testimonio">
                <div class="contenedor-testimonio">
                    <div class="avatar">
                        <img src="https://randomuser.me/api/portraits/men/1.jpg" alt="Cliente 1">
                    </div>
                    <div>
                        <p>"Maximiliano hizo un trabajo increíble en nuestro proyecto. Altamente recomendado."</p>
                        <span class="nombre">**Juan Pérez**</span>
                    </div>
                </div>
            </div>
            <div class="testimonio">
                <div class="contenedor-testimonio">
                    <div class="avatar">
                        <img src="https://randomuser.me/api/portraits/men/2.jpg" alt="Cliente 2">
                    </div>
                    <div>
                        <p>"Muy profesional y excelente comunicación en todo momento. Definitivamente lo contrataría de nuevo."</p>
                        <span class="nombre">**Carlos Díaz**</span>
                    </div>
                </div>
            </div>
            <div class="testimonio">
                <div class="contenedor-testimonio">
                    <div class="avatar">
                        <img src="https://randomuser.me/api/portraits/men/3.jpg" alt="Cliente 3">
                    </div>
                    <div>
                        <p>"El mejor desarrollador con el que he trabajado, siempre en busca de soluciones eficientes."</p>
                        <span class="nombre">**Ricardo Fernández**</span>
                    </div>
                </div>
            </div>
        </div>
    </section>

    <section id="calificar">
        <h2>Califica nuestra página</h2>
        <div class="estrellas">
            <span class="star" onclick="calificar(1)">&#9733;</span>
            <span class="star" onclick="calificar(2)">&#9733;</span>
            <span class="star" onclick="calificar(3)">&#9733;</span>
            <span class="star" onclick="calificar(4)">&#9733;</span>
            <span class="star" onclick="calificar(5)">&#9733;</span>
        </div>
        <div class="comentarios">
            <textarea id="comentario" placeholder="Escribe tu comentario..."></textarea>
            <button onclick="enviarComentario()">Enviar Comentario</button>
        </div>
    </section>

    <section id="contacto">
        <h2>Contacto</h2>
        <form action="gracias.html" method="post">
            <label for="nombre">Nombre:</label>
            <input type="text" id="nombre" name="nombre" required>
            <label for="email">Email:</label>
            <input type="email" id="email" name="email" required>
            <label for="mensaje">Mensaje:</label>
            <textarea id="mensaje" name="mensaje" required></textarea>
            <button type="submit">Enviar</button>
        </form>
    </section>

    <script>
        let carrito = [];
        
        function agregarAlCarrito(nombre, precio) {
            carrito.push({ nombre: nombre, precio: precio });
            mostrarCarrito();
        }
        
        function mostrarCarrito() {
            let carritoContainer = document.getElementById("carrito-container");
            if (carrito.length === 0) {
                carritoContainer.innerHTML = "<p>No hay productos en tu carrito.</p>";
                return;
            }
            carritoContainer.innerHTML = "";
            carrito.forEach(item => {
                let productoElement = document.createElement("div");
                productoElement.classList.add("producto-carrito");
                productoElement.innerHTML = `
                    <p>${item.nombre}</p>
                    <p>$${item.precio}</p>
                `;
                carritoContainer.appendChild(productoElement);
            });
        }
        
        function calificar(estrellas) {
            console.log("Calificación: " + estrellas + " estrellas");
        }

        function enviarComentario() {
            let comentario = document.getElementById("comentario").value;
            console.log("Comentario: " + comentario);
            alert("Gracias por tu comentario.");
        }
    </script>
</body>
</html>
