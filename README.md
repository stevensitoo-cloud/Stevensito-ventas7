[idenx.html](https://github.com/user-attachments/files/33589531/idenx.html)

<!DOCTYPE html>
<html lang="es">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Stevensito Ventas | Archivos y Configs Pro</title>
    <!-- Google Fonts & FontAwesome -->
    <link href="https://fonts.googleapis.com/css2?family=Poppins:wght@300;400;600;700&display=swap" rel="stylesheet">
    <link rel="stylesheet" href="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/6.4.0/css/all.min.css">
    
    <style>
        :root {
            --primary: #8b5cf6;
            --primary-dark: #6d28d9;
            --secondary: #0b0f19;
            --card-bg: #111827;
            --accent: #10b981;
            --text-color: #9ca3af;
            --text-light: #f3f4f6;
            --white: #ffffff;
            --whatsapp: #25d366;
            --telegram: #0088cc;
            --discord: #5865f2;
            --instagram: #e1306c;
        }

        * {
            margin: 0;
            padding: 0;
            box-sizing: border-box;
            font-family: 'Poppins', sans-serif;
        }

        body {
            background-color: var(--secondary);
            color: var(--text-color);
            line-height: 1.6;
        }

        header {
            background-color: rgba(11, 15, 25, 0.95);
            backdrop-filter: blur(10px);
            position: sticky;
            top: 0;
            z-index: 1000;
            border-bottom: 1px solid #1f2937;
        }

        .navbar {
            max-width: 1200px;
            margin: 0 auto;
            padding: 1rem 2rem;
            display: flex;
            justify-content: space-between;
            align-items: center;
        }

        .logo {
            font-size: 1.5rem;
            font-weight: 700;
            color: var(--white);
            text-decoration: none;
            display: flex;
            align-items: center;
            gap: 10px;
        }

        .logo span {
            color: var(--primary);
        }

        .nav-links {
            list-style: none;
            display: flex;
            gap: 1.5rem;
            align-items: center;
        }

        .nav-links a {
            color: var(--text-light);
            text-decoration: none;
            font-weight: 400;
            transition: color 0.3s;
            font-size: 0.95rem;
        }

        .nav-links a:hover {
            color: var(--primary);
        }

        .nav-socials {
            display: flex;
            gap: 1rem;
            margin-left: 1rem;
            border-left: 1px solid #374151;
            padding-left: 1.5rem;
        }

        .nav-socials a {
            color: var(--text-light);
            font-size: 1.1rem;
            transition: transform 0.3s, color 0.3s;
        }

        .nav-socials a:hover {
            transform: scale(1.2);
        }

        .nav-socials .fa-telegram:hover { color: var(--telegram); }
        .nav-socials .fa-discord:hover { color: var(--discord); }
        .nav-socials .fa-instagram:hover { color: var(--instagram); }

        .hero {
            background: linear-gradient(rgba(11, 15, 25, 0.85), rgba(11, 15, 25, 0.95)), url('https://images.unsplash.com/photo-1550745165-9bc0b252726f?auto=format&fit=crop&w=1920&q=80') no-repeat center center/cover;
            color: var(--white);
            text-align: center;
            padding: 7rem 2rem;
            border-bottom: 1px solid #1f2937;
        }

        .hero h1 {
            font-size: 3rem;
            margin-bottom: 1rem;
            font-weight: 700;
        }

        .hero h1 span {
            color: var(--primary);
        }

        .hero p {
            font-size: 1.15rem;
            max-width: 650px;
            margin: 0 auto 2rem;
            color: var(--text-color);
        }

        .btn {
            display: inline-block;
            background-color: var(--primary);
            color: var(--white);
            padding: 0.75rem 2rem;
            border-radius: 8px;
            text-decoration: none;
            font-weight: 600;
            transition: background 0.3s, transform 0.2s;
        }

        .btn:hover {
            background-color: var(--primary-dark);
            transform: translateY(-2px);
        }

        .container {
            max-width: 1200px;
            margin: 0 auto;
            padding: 4rem 2rem;
        }

        .section-title {
            text-align: center;
            font-size: 2.2rem;
            margin-bottom: 0.5rem;
            color: var(--text-light);
        }

        .section-subtitle {
            text-align: center;
            font-size: 1rem;
            margin-bottom: 3rem;
            color: var(--text-color);
        }

        .products-grid {
            display: grid;
            grid-template-columns: repeat(auto-fit, minmax(260px, 1fr));
            gap: 2rem;
        }

        .product-card {
            background: var(--card-bg);
            border: 1px solid #1f2937;
            border-radius: 12px;
            overflow: hidden;
            box-shadow: 0 4px 10px rgba(0,0,0,0.3);
            transition: transform 0.3s, border-color 0.3s;
            display: flex;
            flex-direction: column;
        }

        .product-card:hover {
            transform: translateY(-5px);
            border-color: var(--primary);
        }

        .product-img-container {
            width: 100%;
            height: 160px;
            background: #1f2937;
            display: flex;
            align-items: center;
            justify-content: center;
            position: relative;
        }

        .product-img-container i {
            font-size: 3.5rem;
            color: var(--primary);
        }

        .product-badge {
            position: absolute;
            top: 10px;
            right: 10px;
            background: rgba(139, 92, 246, 0.2);
            color: var(--primary);
            font-size: 0.75rem;
            padding: 4px 10px;
            border-radius: 20px;
            font-weight: 600;
            border: 1px solid var(--primary);
        }

        .product-info {
            padding: 1.5rem;
            display: flex;
            flex-direction: column;
            flex-grow: 1;
        }

        .product-title {
            font-size: 1.2rem;
            color: var(--text-light);
            margin-bottom: 0.5rem;
            font-weight: 600;
        }

        .product-desc {
            font-size: 0.85rem;
            margin-bottom: 1.2rem;
            flex-grow: 1;
        }

        .product-price {
            font-size: 1.35rem;
            font-weight: 700;
            color: var(--accent);
            margin-bottom: 1rem;
        }

        .product-btn {
            width: 100%;
            background-color: var(--primary);
            color: var(--white);
            border: none;
            padding: 0.75rem;
            border-radius: 6px;
            cursor: pointer;
            font-weight: 600;
            transition: background 0.3s;
        }

        .product-btn:hover {
            background-color: var(--primary-dark);
        }

        .modal-overlay {
            display: none;
            position: fixed;
            top: 0;
            left: 0;
            width: 100%;
            height: 100%;
            background: rgba(0, 0, 0, 0.8);
            backdrop-filter: blur(5px);
            z-index: 2000;
            justify-content: center;
            align-items: center;
            padding: 1rem;
        }

        .modal-content {
            background: var(--card-bg);
            border: 1px solid #1f2937;
            border-radius: 14px;
            max-width: 480px;
            width: 100%;
            padding: 2.2rem;
            position: relative;
            box-shadow: 0 20px 25px rgba(0, 0, 0, 0.5);
        }

        .close-modal {
            position: absolute;
            top: 15px;
            right: 20px;
            font-size: 1.6rem;
            color: var(--text-color);
            cursor: pointer;
            transition: color 0.3s;
        }

        .close-modal:hover {
            color: var(--white);
        }

        .modal-content h3 {
            color: var(--text-light);
            margin-bottom: 0.5rem;
            font-size: 1.4rem;
        }

        .modal-content p {
            font-size: 0.9rem;
            margin-bottom: 1rem;
        }

        .bank-list {
            background: #0b0f19;
            border: 1px solid #1f2937;
            border-radius: 8px;
            padding: 1rem;
            margin: 1rem 0;
        }

        .bank-item {
            margin-bottom: 0.8rem;
            font-size: 0.9rem;
        }

        .bank-item:last-child {
            margin-bottom: 0;
        }

        .bank-item strong {
            color: var(--text-light);
        }

        .titular-box {
            font-size: 0.85rem;
            color: var(--accent);
            background: rgba(16, 185, 129, 0.1);
            padding: 10px;
            border-radius: 6px;
            border: 1px solid var(--accent);
            text-align: center;
            margin-top: 1rem;
            font-weight: 600;
        }

        .whatsapp-proof-btn {
            display: flex;
            align-items: center;
            justify-content: center;
            gap: 10px;
            width: 100%;
            background-color: var(--whatsapp);
            color: #ffffff;
            text-decoration: none;
            padding: 0.85rem;
            border-radius: 8px;
            font-weight: 600;
            margin-top: 1.2rem;
            transition: background 0.3s;
        }

        .whatsapp-proof-btn:hover {
            background-color: #1ebe5d;
        }

        footer {
            background-color: #080b12;
            border-top: 1px solid #1f2937;
            color: var(--text-color);
            text-align: center;
            padding: 3.5rem 2rem;
            margin-top: 4rem;
        }

        .support-info {
            font-size: 1.1rem;
            color: var(--text-light);
            margin-bottom: 1.5rem;
        }

        .support-info i {
            color: var(--whatsapp);
            margin-right: 8px;
        }

        .social-icons {
            display: flex;
            justify-content: center;
            gap: 1.5rem;
            margin-bottom: 1.5rem;
        }

        .social-icons a {
            background: #111827;
            border: 1px solid #1f2937;
            width: 45px;
            height: 45px;
            border-radius: 50%;
            display: flex;
            align-items: center;
            justify-content: center;
            color: var(--text-light);
            font-size: 1.2rem;
            transition: all 0.3s;
        }

        .social-icons a.wa:hover { background-color: var(--whatsapp); border-color: var(--whatsapp); color: #fff; }
        .social-icons a.tg:hover { background-color: var(--telegram); border-color: var(--telegram); color: #fff; }
        .social-icons a.dc:hover { background-color: var(--discord); border-color: var(--discord); color: #fff; }
        .social-icons a.ig:hover { background-color: var(--instagram); border-color: var(--instagram); color: #fff; }

        footer h3 {
            color: var(--text-light);
            margin-bottom: 0.5rem;
        }

        footer p {
            font-size: 0.9rem;
            margin-top: 1rem;
        }

        @media (max-width: 768px) {
            .navbar {
                flex-direction: column;
                gap: 1rem;
            }
            .nav-socials {
                border-left: none;
                padding-left: 0;
                border-top: 1px solid #374151;
                padding-top: 0.5rem;
            }
        }
    </style>
</head>
<body>

    <header>
        <nav class="navbar">
            <a href="#" class="logo"><i class="fas fa-file-code"></i>Stevensito<span>Ventas</span></a>
            <ul class="nav-links">
                <li><a href="#">Inicio</a></li>
                <li><a href="#catalogo">Catálogo</a></li>
                <li><a href="#soporte">Soporte</a></li>
                <div class="nav-socials">
                    <a href="https://t.me/stvnsxsitoroot" target="_blank" title="Telegram"><i class="fab fa-telegram"></i></a>
                    <a href="https://discord.gg/bEMHqv3hd" target="_blank" title="Discord"><i class="fab fa-discord"></i></a>
                    <a href="https://www.instagram.com/stevensxtoo?xtok=bGw0dmZsNGFmbDN6&utm_source=qr" target="_blank" title="Instagram"><i class="fab fa-instagram"></i></a>
                </div>
            </ul>
        </nav>
    </header>

    <section class="hero">
        <h1>Archivos y Scripts Exclusivos en <span>Stevensito Ventas</span></h1>
        <p>Mejora tu precisión y rendimiento con configuraciones avanzadas garantizadas.</p>
        <a href="#catalogo" class="btn">Ver Catálogo</a>
    </section>

    <main class="container" id="catalogo">
        <h2 class="section-title">Catálogo de Archivos</h2>
        <p class="section-subtitle">Precios desde $20 hasta $35 dólares</p>
        
        <div class="products-grid">
            <div class="product-card">
                <div class="product-img-container">
                    <span class="product-badge">$25.00</span>
                    <i class="fas fa-crosshairs"></i>
                </div>
                <div class="product-info">
                    <h3 class="product-title">Aim Cuello</h3>
                    <p class="product-desc">Archivo de optimización calibrado exactamente a la altura del cuello.</p>
                    <div class="product-price">$25.00 USD</div>
                    <button class="product-btn" onclick="abrirModal('Aim Cuello')">Comprar Archivo</button>
                </div>
            </div>

            <div class="product-card">
                <div class="product-img-container">
                    <span class="product-badge">$20.00</span>
                    <i class="fas fa-robot"></i>
                </div>
                <div class="product-info">
                    <h3 class="product-title">Aim Body</h3>
                    <p class="product-desc">Configuración estable y fluida para control general de movimientos.</p>
                    <div class="product-price">$20.00 USD</div>
                    <button class="product-btn" onclick="abrirModal('Aim Body')">Comprar Archivo</button>
                </div>
            </div>

            <div class="product-card">
                <div class="product-img-container">
                    <span class="product-badge">$22.00</span>
                    <i class="fas fa-bolt"></i>
                </div>
                <div class="product-info">
                    <h3 class="product-title">Aim Drag</h3>
                    <p class="product-desc">Asistencia de arrastre suave para mayor precisión al deslizar la mira.</p>
                    <div class="product-price">$22.00 USD</div>
                    <button class="product-btn" onclick="abrirModal('Aim Drag')">Comprar Archivo</button>
                </div>
            </div>

            <div class="product-card">
                <div class="product-img-container">
                    <span class="product-badge">$35.00</span>
                    <i class="fas fa-bullseye"></i>
                </div>
                <div class="product-info">
                    <h3 class="product-title">Aim Head</h3>
                    <p class="product-desc">Script de gama alta enfocado al enfoque directo a la cabeza.</p>
                    <div class="product-price">$35.00 USD</div>
                    <button class="product-btn" onclick="abrirModal('Aim Head')">Comprar Archivo</button>
                </div>
            </div>

            <div class="product-card">
                <div class="product-img-container">
                    <span class="product-badge">$30.00</span>
                    <i class="fas fa-cube"></i>
                </div>
                <div class="product-info">
                    <h3 class="product-title">Hologramas</h3>
                    <p class="product-desc">Paquete de efectos visuales personalizados de alta resolución.</p>
                    <div class="product-price">$30.00 USD</div>
                    <button class="product-btn" onclick="abrirModal('Hologramas')">Comprar Archivo</button>
                </div>
            </div>
        </div>
    </main>

    <div class="modal-overlay" id="modalBanco">
        <div class="modal-content">
            <span class="close-modal" onclick="cerrarModal()">&times;</span>
            <h3>Datos Bancarios para Pago</h3>
            <p>Realiza tu transferencia o depósito a cualquiera de nuestras cuentas:</p>
            
            <div class="bank-list">
                <div class="bank-item">
                    <strong>BHD:</strong> 39485700011
                </div>
                <div class="bank-item">
                    <strong>Banreservas:</strong> 9607568789 (Cuenta de Ahorro)
                </div>
                <div class="bank-item">
                    <strong>Popular:</strong> 859867871
                </div>
            </div>

            <div class="titular-box">
                Titular: Sr. Richard Steven De Los Santos Beltrán
            </div>
            
            <a id="whatsappBtnLink" href="https://wa.me/18297730909" target="_blank" class="whatsapp-proof-btn">
                <i class="fab fa-whatsapp" style="font-size: 1.2rem;"></i> Enviar Comprobante por WhatsApp
            </a>
        </div>
    </div>

    <footer id="soporte">
        <div class="support-info">
            <i class="fas fa-phone-alt"></i> Soporte y WhatsApp: <strong>829-773-0909</strong>
        </div>
        <div class="social-icons">
            <a href="https://wa.me/18297730909" target="_blank" class="wa" title="WhatsApp"><i class="fab fa-whatsapp"></i></a>
            <a href="https://t.me/stvnsxsitoroot" target="_blank" class="tg" title="Telegram"><i class="fab fa-telegram"></i></a>
            <a href="https://discord.gg/bEMHqv3hd" target="_blank" class="dc" title="Discord"><i class="fab fa-discord"></i></a>
            <a href="https://www.instagram.com/stevensxtoo?xtok=bGw0dmZsNGFmbDN6&utm_source=qr" target="_blank" class="ig" title="Instagram"><i class="fab fa-instagram"></i></a>
        </div>
        <h3>Stevensito Ventas</h3>
        <p>&copy; 2026 Stevensito Ventas. Todos los derechos reservados.</p>
    </footer>

    <script>
        function abrirModal(nombreProducto) {
            document.getElementById('modalBanco').style.display = 'flex';
            let mensaje = "Hola, acabo de realizar el pago para el archivo: *" + nombreProducto + "*. Aquí adjunto mi comprobante:";
            let urlWhatsApp = "https://wa.me/18297730909?text=" + encodeURIComponent(mensaje);
            document.getElementById('whatsappBtnLink').setAttribute('href', urlWhatsApp);
        }

        function cerrarModal() {
            document.getElementById('modalBanco').style.display = 'none';
        }

        window.onclick = function(event) {
            let modal = document.getElementById('modalBanco');
            if (event.target == modal) {
                modal.style.display = 'none';
            }
        }
    </script>
</body>
</html>
