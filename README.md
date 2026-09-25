 <!DOCTYPE html>
<html lang="es">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Propuesta Comercial - Banorte Móvil</title>
    <style>
        :root {
            --banorte-red: #EB0029;
            --banorte-dark-red: #B3001F;
            --banorte-gray: #5f6368;
            --banorte-bg: #F4F6F8;
            --text-color: #2D3142;
        }

        * {
            box-sizing: border-box;
            margin: 0;
            padding: 0;
            font-family: 'Segoe UI', Tahoma, Geneva, Verdana, sans-serif;
        }

        body {
            background-color: var(--banorte-bg);
            color: var(--text-color);
            line-height: 1.6;
        }

        /* Header / Navbar */
        header {
            background-color: #ffffff;
            padding: 15px 5%;
            display: flex;
            justify-content: space-between;
            align-items: center;
            box-shadow: 0 2px 10px rgba(0,0,0,0.08);
            position: sticky;
            top: 0;
            z-index: 1000;
        }

        .logo img {
            height: 38px;
            width: auto;
            display: block;
        }

        .badge-nav {
            background-color: var(--banorte-red);
            color: white;
            padding: 6px 14px;
            border-radius: 20px;
            font-size: 0.85rem;
            font-weight: 600;
        }

        /* Hero Section */
        .hero {
            background: linear-gradient(135deg, var(--banorte-red) 0%, var(--banorte-dark-red) 100%);
            color: white;
            padding: 60px 5%;
            display: flex;
            align-items: center;
            justify-content: space-between;
            flex-wrap: wrap;
            gap: 40px;
            min-height: 480px;
        }

        .hero-content {
            flex: 1;
            min-width: 300px;
        }

        .hero-title {
            font-size: 2.8rem;
            font-weight: 800;
            margin-bottom: 15px;
            line-height: 1.2;
        }

        .hero-subtitle {
            font-size: 1.2rem;
            margin-bottom: 25px;
            opacity: 0.95;
            max-width: 600px;
        }

        .hero-tags {
            display: flex;
            gap: 10px;
            flex-wrap: wrap;
        }

        .hero-tag {
            background: rgba(255, 255, 255, 0.2);
            backdrop-filter: blur(5px);
            padding: 6px 16px;
            border-radius: 30px;
            font-size: 0.9rem;
            border: 1px solid rgba(255, 255, 255, 0.3);
        }

        .hero-image {
            flex: 1;
            min-width: 280px;
            display: flex;
            justify-content: center;
        }

        .hero-image img {
            max-width: 100%;
            max-height: 380px;
            border-radius: 16px;
            box-shadow: 0 15px 30px rgba(0,0,0,0.3);
            object-fit: cover;
        }

        /* Container & Cards Section */
        .container {
            max-width: 1200px;
            margin: 40px auto;
            padding: 0 20px;
        }

        .section-title {
            text-align: center;
            font-size: 1.8rem;
            color: var(--banorte-dark-red);
            margin-bottom: 30px;
            position: relative;
        }

        .section-title::after {
            content: '';
            width: 60px;
            height: 4px;
            background-color: var(--banorte-red);
            display: block;
            margin: 8px auto 0;
            border-radius: 2px;
        }

        /* Grid Metrics */
        .metrics-grid {
            display: grid;
            grid-template-columns: repeat(auto-fit, minmax(240px, 1fr));
            gap: 20px;
            margin-bottom: 50px;
        }

        .metric-card {
            background: white;
            padding: 25px;
            border-radius: 12px;
            box-shadow: 0 4px 15px rgba(0,0,0,0.05);
            border-left: 5px solid var(--banorte-red);
            transition: transform 0.2s ease;
        }

        .metric-card:hover {
            transform: translateY(-5deg);
        }

        .metric-card h4 {
            color: var(--banorte-gray);
            font-size: 0.9rem;
            text-transform: uppercase;
            letter-spacing: 0.5px;
            margin-bottom: 8px;
        }

        .metric-card p {
            font-size: 1.6rem;
            font-weight: 700;
            color: var(--text-color);
        }

        /* Two Column Layout */
        .two-column {
            display: grid;
            grid-template-columns: 1fr 1fr;
            gap: 30px;
            margin-bottom: 50px;
        }

        @media (max-width: 768px) {
            .two-column {
                grid-template-columns: 1fr;
            }
        }

        .info-box {
            background: white;
            padding: 30px;
            border-radius: 12px;
            box-shadow: 0 4px 15px rgba(0,0,0,0.05);
        }

        .info-box h3 {
            color: var(--banorte-red);
            margin-bottom: 15px;
            font-size: 1.3rem;
        }

        .info-box ul {
            list-style: none;
        }

        .info-box li {
            position: relative;
            padding-left: 25px;
            margin-bottom: 12px;
        }

        .info-box li::before {
            content: '✓';
            position: absolute;
            left: 0;
            color: var(--banorte-red);
            font-weight: bold;
        }

        .sec-image img {
            width: 100%;
            height: 250px;
            object-fit: cover;
            border-radius: 12px;
            margin-top: 15px;
        }

        /* Footer */
        footer {
            background-color: #1A1A1A;
            color: white;
            text-align: center;
            padding: 20px;
            font-size: 0.9rem;
            margin-top: 50px;
        }
    </style>
</head>
<body>

    <!-- Header -->
    <header>
        <div class="logo">
            <!-- Imagen 1: Logo Banorte -->
            <img src="Captura de pantalla 2026-09-25 a la(s) 10.50.16 a.m._2.png" alt="Logo Banorte">
        </div>
        <div class="badge-nav">Propuesta Estratégica 2026</div>
    </header>

    <!-- Hero Section -->
    <section class="hero">
        <div class="hero-content">
            <h1 class="hero-title">Banorte Móvil</h1>
            <p class="hero-subtitle">Estrategia integral de adquisición e instalación de la aplicación (CPI) mediante optimización avanzada de audiencias y canales digitales.</p>
            <div class="hero-tags">
                <span class="hero-tag">🎯 Objetivo: App Install / CPI</span>
                <span class="hero-tag">🇲🇽 Cobertura: Nacional</span>
                <span class="hero-tag">💡 CPC: $9.00 MXN</span>
            </div>
        </div>
        <div class="hero-image">
            <!-- Imagen 2: Hero Style User Mobile -->
            <img src="Captura de pantalla 2026-09-25 a la(s) 10.51.38 a.m._2.jpg" alt="Usuario Banorte Móvil">
        </div>
    </section>

    <!-- Main Container -->
    <div class="container">

        <!-- Objetivo General -->
        <h2 class="section-title">Objetivo de la Campaña</h2>
        <div class="info-box" style="margin-bottom: 40px; text-align: center;">
            <p style="font-size: 1.15rem; max-width: 900px; margin: 0 auto; color: #444;">
                Impulsar el crecimiento y la adopción digital de la plataforma <strong>Banorte Móvil</strong> a nivel nacional, optimizando el costo por adquisición mediante la ejecución de un mix de formatos de alto rendimiento orientados a la conversión e instalación efectiva.
            </p>
        </div>

        <!-- IndicadoresClave / Premisas -->
        <h2 class="section-title">Parámetros Comerciales</h2>
        <div class="metrics-grid">
            <div class="metric-card">
                <h4>Costo Por Clic (CPC)</h4>
                <p>$9.00 MXN</p>
            </div>
            <div class="metric-card">
                <h4>Alcance Geo</h4>
                <p>Nacional (México)</p>
            </div>
            <div class="metric-card">
                <h4>Modelo de Compra</h4>
                <p>CPI / App Install</p>
            </div>
            <div class="metric-card">
                <h4>Tecnología</h4>
                <p>Machine Learning</p>
            </div>
        </div>

        <!-- Estrategia y Formatos -->
        <div class="two-column">
            <!-- Columna Formatos -->
            <div class="info-box">
                <h3>Formatos de Medios Utilizados</h3>
                <ul>
                    <li><strong>Native:</strong> Integración orgáñica en plataformas de contenido de alto impacto.</li>
                    <li><strong>Display:</strong> Banners dinámicos optimizados para conversión.</li>
                    <li><strong>Email Marketing:</strong> Impacto directo a bases segmentadas de valor.</li>
                    <li><strong>Push Notifications:</strong> Alertas dinámicas orientadas a la descarga inmediata.</li>
                </ul>
            </div>

            <!-- Columna Medición y Seguridad -->
            <div class="info-box">
                <h3>Estrategia, Medición y Seguridad</h3>
                <ul>
                    <li><strong>Optimización Operativa:</strong> Ajuste dinámico de pujas mediante Machine Learning.</li>
                    <li><strong>Validación de Tráfico:</strong> Control de calidad e implementación de mecanismos anti-fraude.</li>
                    <li><strong>Medición Multiplataforma:</strong> Atribución precisa en entornos iOS y Android.</li>
                </ul>
                <!-- Imagen 3: Ciberseguridad / Tecnología -->
                <img src="Captura de pantalla 2026-09-25 a la(s) 10.52.37 a.m._2.jpg" alt="Seguridad Digital y Medición" class="sec-image">
            </div>
        </div>

    </div>

    <!-- Footer -->
    <footer>
        <p>&copy; 2026 Propuesta de Estrategia Digital — Banorte Móvil. Todos los derechos reservados.</p>
    </footer>

</body>
</html>
