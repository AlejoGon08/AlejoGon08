<!DOCTYPE html>
<html lang="es">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Aurora Arquitectura</title>
    <style>
        body {
            font-family: Arial, sans-serif;
            background-color: #f0f0f0;
            color: #333;
            margin: 0;
            padding: 0;
        }
        header {
            display: flex;
            align-items: center;
            background-color: #ccc;
            padding: 10px;
        }
        header img {
            height: 50px;
            margin-right: 10px;
        }
        nav {
            margin-left: auto;
        }
        nav button {
            background-color: transparent;
            border: none;
            padding: 10px;
            cursor: pointer;
            font-size: 16px;
        }
        .hidden {
            display: none;
        }
        .project {
            margin: 20px;
            text-align: center;
        }
        .project img {
            max-width: 100%;
            height: auto;
            cursor: pointer;
        }
        .description {
            display: none;
            margin-top: 10px;
        }
        footer {
            background-color: #ccc;
            padding: 10px;
            text-align: center;
        }
    </style>
    <script>
        function toggleSection(id) {
            document.querySelectorAll('.hidden').forEach(el => el.style.display = 'none');
            document.getElementById(id).style.display = 'block';
        }
        function toggleDescription(id) {
            var desc = document.getElementById(id);
            desc.style.display = desc.style.display === 'block' ? 'none' : 'block';
        }
    </script>
</head>
<body>
    <header>
        <img src="logo.png" alt="Aurora Arquitectura">
        <h1>Aurora Arquitectura</h1>
        <nav>
            <button onclick="toggleSection('proyectos')">Proyectos</button>
            <button onclick="toggleSection('quienes-somos')">Quiénes Somos</button>
        </nav>
    </header>
    
    <div id="inicio" style="text-align: center; font-family: 'Poppins', sans-serif; color: #ffffff; background: linear-gradient(to bottom, rgba(0, 0, 0, 0.6), rgba(0, 0, 0, 0.9)), url('1730147544977.jpg'); background-size: cover; background-position: center; padding: 100px 20px;">
    <h2 style="font-size: 3rem; font-weight: 700; text-transform: uppercase; margin-bottom: 10px;">Bienvenidos a Aurora Arquitectura</h2>
    <p style="font-size: 1.2rem; max-width: 800px; margin: auto; line-height: 1.8;">
        En <strong>Aurora Arquitectura</strong>, creemos que cada espacio tiene el poder de transmitir sensaciones, contar historias y mejorar la vida de quienes lo habitan. Nuestro enfoque se centra en el diseño de interiores y la arquitectura comercial, creando ambientes que combinan funcionalidad, estética y una identidad única.
    </p>
    <p style="font-size: 1.2rem; max-width: 800px; margin: auto; line-height: 1.8; margin-top: 15px;">
        Buscamos el equilibrio perfecto entre belleza y funcionalidad, adaptándonos a cada necesidad para dar vida a espacios que no solo se ven bien, sino que también se sienten bien. 
        <br><br>
        <em>Diseño que inspira, transforma y trasciende.</em>
    </p>
</div>

    </div>
    
    <div id="proyectos" class="hidden">
    <div class="project">
        <h3 onclick="toggleDescription('desc1')" style="cursor: pointer; font-size: 1.5rem; color: #333; text-transform: uppercase; margin-bottom: 10px;">Refugio Urbano</h3>
        <img src="gastrobar-segundo-nivel.png" alt="Refugio Urbano" onclick="toggleDescription('desc1')">
        <img src="gastrobar-primer-nivel.png" alt="Refugio Urbano" onclick="toggleDescription('desc1')">
        <p id="desc1" class="description" style="display: none; font-size: 1.1rem; color: #555; margin-top: 10px;">
            Diseño de un gastrobar que fusiona la modernidad con el ambiente acogedor de la ciudad. Espacios cuidadosamente pensados para una experiencia única.
        </p>
    </div>
    <div class="project">
        <h3 onclick="toggleDescription('desc2')" style="cursor: pointer; font-size: 1.5rem; color: #333; text-transform: uppercase; margin-bottom: 10px;">Diseños de Interior</h3>
        <img src="sala-gris.png" alt="Diseños de Interior" onclick="toggleDescription('desc2')">
        <img src="sala-exterior.jpeg" alt="Diseños de Interior" onclick="toggleDescription('desc2')">
        <p id="desc2" class="description" style="display: none; font-size: 1.1rem; color: #555; margin-top: 10px;">
            Transformación de interiores para crear ambientes funcionales y estéticamente agradables, optimizando cada rincón según las necesidades de los usuarios.
        </p>
    </div>
    <div class="project">
        <h3 onclick="toggleDescription('desc3')" style="cursor: pointer; font-size: 1.5rem; color: #333; text-transform: uppercase; margin-bottom: 10px;">Elixir Urbano</h3>
        <img src="gastrobar-exterior-noche.jpeg" alt="Elixir Urbano" onclick="toggleDescription('desc3')">
        <img src="gastrobar-exterior-noche2.jpeg" alt="Elixir Urbano" onclick="toggleDescription('desc3')">
        <img src="gastrobar-exterior-dia.jpeg" alt="Elixir Urbano" onclick="toggleDescription('desc3')">
        <p id="desc3" class="description" style="display: none; font-size: 1.1rem; color: #555; margin-top: 10px;">
            Un concepto de gastrobar en un entorno urbano que destaca por su diseño contemporáneo, creando un lugar perfecto tanto de día como de noche.
        </p>
    </div>
    <div class="project">
        <h3 onclick="toggleDescription('desc4')" style="cursor: pointer; font-size: 1.5rem; color: #333; text-transform: uppercase; margin-bottom: 10px;">Cabañas y Glampings</h3>
        <img src="CABAÑA.jpeg" alt="Cabañas y Glampings" onclick="toggleDescription('desc4')">
        <p id="desc4" class="description" style="display: none; font-size: 1.1rem; color: #555; margin-top: 10px;">
            Diseño de cabañas y glampings que fusionan confort y naturaleza, creando un refugio perfecto para quienes buscan desconectarse en un entorno natural.
        </p>
    </div>
</div>

        </div>
    </div>
    
    <div id="quienes-somos" class="hidden">
        <h2>Quiénes Somos</h2>
        <p>XXXXXXXXXX (Misión y visión)</p>
    </div>
    
    <footer>
        <h3>Contacto</h3>
        <p>Tel: 3195361962</p>
        <p>Email: arq.alejandrogon@gmail.com</p>
        <p>Instagram: @aurora.arquitectura</p>
    </footer>
</body>
</html>
