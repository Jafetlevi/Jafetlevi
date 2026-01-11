<!DOCTYPE html>
<html lang="es">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Imagen Personal | Doble Filo</title>
    <link href="https://fonts.googleapis.com/css2?family=Cormorant+Garamond:wght@300;400;600&family=Montserrat:wght@100;300;400&display=swap" rel="stylesheet">
    <style>
        :root { 
            --oro-viejo: #c5a059; 
            --negro-ebano: #050505; 
            --negro-suave: #0f0f0f;
            --blanco-seda: #f4f4f4; 
        }

        body { 
            background: var(--negro-ebano); 
            color: var(--blanco-seda); 
            font-family: 'Montserrat', sans-serif; 
            margin: 0; 
            line-height: 1.6;
        }

        /* NAVEGACIÓN SUPERIOR */
        .nav-back {
            padding: 30px 5%;
            display: flex;
            justify-content: space-between;
            align-items: center;
            border-bottom: 1px solid rgba(197, 160, 89, 0.1);
        }

        .nav-back a {
            color: var(--oro-viejo);
            text-decoration: none;
            font-size: 0.7em;
            letter-spacing: 3px;
            text-transform: uppercase;
            border: 1px solid var(--oro-viejo);
            padding: 8px 15px;
            transition: 0.3s;
        }

        .nav-back a:hover { background: var(--oro-viejo); color: black; }

        /* CABECERA DE LA PÁGINA */
        .section-header {
            text-align: center;
            padding: 60px 5% 40px;
        }

        .section-header span {
            color: var(--oro-viejo);
            letter-spacing: 10px;
            font-size: 0.7em;
            text-transform: uppercase;
            display: block;
            margin-bottom: 10px;
        }

        .section-header h1 {
            font-family: 'Cormorant Garamond', serif;
            font-size: 4em;
            margin: 0;
            font-weight: 300;
        }

        /* CUADRÍCULA DE SERVICIOS (3 BLOQUES) */
        .grid-servicios {
            display: grid;
            grid-template-columns: repeat(auto-fit, minmax(320px, 1fr));
            gap: 1px;
            background: rgba(197, 160, 89, 0.1); /* Color de la línea divisoria */
            border-top: 1px solid rgba(197, 160, 89, 0.1);
            border-bottom: 1px solid rgba(197, 160, 89, 0.1);
            margin-bottom: 80px;
        }

        .bloque {
            background: var(--negro-ebano);
            padding: 60px 45px;
            transition: 0.5s ease;
        }

        .bloque:hover { background: var(--negro-suave); }

        .bloque h2 {
            font-family: 'Cormorant Garamond', serif;
            font-size: 2.5em;
            color: var(--oro-viejo);
            margin-bottom: 35px;
            font-weight: 400;
            border-bottom: 1px solid rgba(197, 160, 89, 0.2);
            padding-bottom: 15px;
        }

        /* LISTADO INTERNO */
        .servicio-info {
            margin-bottom: 30px;
        }

        .servicio-info h3 {
            font-size: 0.85em;
            letter-spacing: 2px;
            text-transform: uppercase;
            margin-bottom: 8px;
            color: var(--blanco-seda);
        }

        .servicio-info p {
            font-size: 0.8em;
            color: #777;
            margin-bottom: 12px;
            font-weight: 300;
        }

        /* BOTONES DE ENLACE */
        .btn-link {
            display: inline-block;
            color: var(--oro-viejo);
            text-decoration: none;
            font-size: 0.65em;
            letter-spacing: 2px;
            border-bottom: 1px solid var(--oro-viejo);
            padding-bottom: 3px;
            transition: 0.3s;
        }

        .btn-link:hover { color: white; border-color: white; }

        @media (max-width: 768px) {
            .section-header h1 { font-size: 2.8em; }
            .grid-servicios { gap: 20px; background: transparent; }
        }
    </style>
</head>
<body>

    <nav class="nav-back">
        <div style="font-family: 'Cormorant Garamond'; letter-spacing: 5px; font-size: 1.1em;">DOBLE FILO</div>
        <a href="index.html">← VOLVER</a>
    </nav>

    <header class="section-header">
        <span>FILO I</span>
        <h1>Imagen Personal</h1>
    </header>

    <main class="grid-servicios">
        
        <section class="bloque">
            <h2>Boutique</h2>
            <div class="servicio-info">
                <h3>Cortes de Dama</h3>
                <p>Diseño de autor basado en proporciones áureas y visajismo.</p>
                <a href="cortes-dama.html" class="btn-link">VER TENDENCIAS →</a>
            </div>
            <div class="servicio-info">
                <h3>Barbería</h3>
                <p>Estructuras clásicas y modernas con técnicas de perfilado superior.</p>
                <a href="barberia.html" class="btn-link">VER CATÁLOGO →</a>
            </div>
        </section>

        <section class="bloque">
            <h2>Servicios</h2>
            <div class="servicio-info">
                <h3>Arquitectura de Cejas</h3>
                <p>Rediseño de mirada mediante análisis morfológico.</p>
            </div>
            <div class="servicio-info">
                <h3>Colorimetría</h3>
                <p>Estrategias de color avanzada y corrección técnica.</p>
            </div>
            <div class="servicio-info">
                <h3>Visajismo Facial</h3>
                <p>Perfilado de rostro y asesoría estructural personalizada.</p>
            </div>
        </section>

        <section class="bloque">
            <h2>Cuidados</h2>
            <div class="servicio-info">
                <h3>Detox Capilar</h3>
                <p>Tratamiento de purificación y salud del cuero cabelludo.</p>
            </div>
            <div class="servicio-info">
                <h3>Masajes</h3>
                <p>Terapia de relajación craneal y estimulación sensorial.</p>
            </div>
            <div class="servicio-info">
                <h3>Tratamientos</h3>
                <p>Hidratación profunda y sellado térmico con activos premium.</p>
            </div>
        </section>

    </main>

    <footer style="text-align:center; padding: 40px; color:#222; font-size:0.6em; letter-spacing:4px;">
        DOBLE FILO STUDIO | ALTA PELUQUERÍA & ESTRATEGIA
    </footer>

</body>
</html>
