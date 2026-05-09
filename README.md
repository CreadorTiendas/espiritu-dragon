<!DOCTYPE html>
<html lang="es">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0, user-scalable=yes">
    <title>Espíritu del Dragón - Sanación Ancestral</title>
    <style>
        * { margin: 0; padding: 0; box-sizing: border-box; }
        body { font-family: 'Segoe UI', Tahoma, Geneva, Verdana, sans-serif; background: #fdfaf6; color: #2a2a2a; line-height: 1.6; }
        header { background: #4a2c2c; color: #e6c8a0; padding: 2rem; text-align: center; border-bottom: 4px solid #b8860b; }
        .container { max-width: 1200px; margin: auto; padding: 2rem; }
        .estadisticas { display: flex; gap: 2rem; flex-wrap: wrap; justify-content: center; margin-bottom: 2rem; }
        .tarjeta-estadistica { background: white; border-radius: 20px; padding: 1rem; flex: 1; min-width: 120px; text-align: center; box-shadow: 0 2px 5px rgba(0,0,0,0.1);}
        .numero { font-size: 2rem; font-weight: bold; color: #b8860b; }
        .servicios, .paquetes { display: flex; gap: 2rem; flex-wrap: wrap; justify-content: center; margin-bottom: 3rem; }
        .card { background: white; border-radius: 20px; padding: 1.5rem; flex: 1; min-width: 280px; max-width: 320px; box-shadow: 0 10px 20px rgba(0,0,0,0.05); border-top: 4px solid #b8860b; text-align: center; }
        .precio { font-size: 2rem; color: #4a2c2c; font-weight: bold; margin: 1rem 0; background: #fdfaf6; display: inline-block; padding: 0.3rem 1rem; border-radius: 40px; }
        .btn { display: inline-block; background: #b8860b; color: white; padding: 0.8rem 1rem; border-radius: 50px; text-decoration: none; font-weight: bold; margin-top: 1rem; width: 100%; text-align: center; cursor: pointer; border: none; }
        footer { background: #2a2a2a; color: #e6c8a0; text-align: center; padding: 2rem; margin-top: 2rem; }
        @media (max-width: 768px) { .servicios, .paquetes { flex-direction: column; align-items: center; } }
    </style>
</head>
<body>
    <header>
        <h1>🐉 ESPÍRITU DEL DRAGÓN</h1>
        <p>Sanación ancestral con aromaterapia, acupuntura y moxibustión</p>
    </header>
    <div class="container">
        <div class="estadisticas">
            <div class="tarjeta-estadistica"><h3>👁️ Visitas</h3><div class="numero" id="visitas">0</div></div>
            <div class="tarjeta-estadistica"><h3>💬 Consultas</h3><div class="numero" id="consultas">0</div></div>
            <div class="tarjeta-estadistica"><h3>💰 Cotizaciones</h3><div class="numero" id="cotizaciones">0</div></div>
        </div>
        
        <h2>🌿 Nuestros Servicios</h2>
        <div class="servicios">
            <div class="card"><h3>Aromaterapia</h3><div class="precio">$390 MXN</div><ul><li>🌼 Aceites esenciales puros</li><li>🕯️ Consulta personalizada</li><li>✨ Equilibrio emocional</li></ul><button class="btn" onclick="registrarCotizacion('Aromaterapia')">📲 Contratar</button></div>
            <div class="card"><h3>Acupuntura</h3><div class="precio">$550 MXN</div><ul><li>📍 Puntos energéticos</li><li>⚡ Alivio del dolor</li><li>🍃 Sin dolor</li></ul><button class="btn" onclick="registrarCotizacion('Acupuntura')">📲 Contratar</button></div>
            <div class="card"><h3>Moxibustión</h3><div class="precio">$680 MXN</div><ul><li>🔥 Terapia de calor</li><li>🌿 Con hierbas medicinales</li><li>💪 Fortalece el Qi</li></ul><button class="btn" onclick="registrarCotizacion('Moxibustión')">📲 Contratar</button></div>
            <div class="card"><h3>Masaje Terapéutico</h3><div class="precio">$550 MXN</div><ul><li>💆‍♂️ Descontracturante</li><li>🕊️ Relajante profundo</li><li>🔄 Mejora circulación</li></ul><button class="btn" onclick="registrarCotizacion('Masaje')">📲 Contratar</button></div>
        </div>

        <h2>🎁 Paquetes Especiales</h2>
        <div class="paquetes">
            <div class="card"><h3>Bienestar Básico</h3><div class="precio">$800 MXN</div><ul><li>✨ Aromaterapia + Masaje</li><li>🎯 Ideal para estrés</li><li>🕒 Duración: 90 min</li></ul><button class="btn" onclick="registrarCotizacion('Bienestar Básico')">📲 Contratar</button></div>
            <div class="card"><h3>Equilibrio Energético</h3><div class="precio">$950 MXN</div><ul><li>⚡ Acupuntura + Moxibustión</li><li>🎯 Para fatiga crónica</li><li>🕒 Duración: 2 horas</li></ul><button class="btn" onclick="registrarCotizacion('Equilibrio Energético')">📲 Contratar</button></div>
            <div class="card"><h3>Desintoxicación Profunda</h3><div class="precio">$1,200 MXN</div><ul><li>🔥 Terapia Kombinada</li><li>🎯 Dolor muscular intenso</li><li>🕒 Duración: 2.5 horas</li></ul><button class="btn" onclick="registrarCotizacion('Desintoxicación Profunda')">📲 Contratar</button></div>
            <div class="card"><h3>Cuidado Integral</h3><div class="precio">$1,900 MXN</div><ul><li>🏆 4 servicios juntos</li><li>🎯 Sanación completa</li><li>🕒 Duración: 3 horas</li></ul><button class="btn" onclick="registrarCotizacion('Cuidado Integral')">📲 Contratar</button></div>
        </div>
    </div>
    <footer>
        <p>📧 contacto@espiritudragon.com | 📞 52 777 910 7055</p>
        <p>© 2026 Espíritu del Dragón - Sanación ancestral</p>
    </footer>

    <!-- Tidio Chat (Lyro AI) - Funciona 100% -->
    <script src="//code.tidio.co/turocovxhshqbvu6tzomxcxuaoiejo4m.js" async></script>

    <script>
        let visitas = localStorage.getItem('visitas_dragon') ? parseInt(localStorage.getItem('visitas_dragon')) : 0;
        let consultas = localStorage.getItem('consultas_dragon') ? parseInt(localStorage.getItem('consultas_dragon')) : 0;
        let cotizaciones = localStorage.getItem('cotizaciones_dragon') ? parseInt(localStorage.getItem('cotizaciones_dragon')) : 0;
        visitas++; localStorage.setItem('visitas_dragon', visitas);
        document.getElementById('visitas').innerText = visitas;
        document.getElementById('consultas').innerText = consultas;
        document.getElementById('cotizaciones').innerText = cotizaciones;
        
        window.registrarCotizacion = function(pack) { cotizaciones++; localStorage.setItem('cotizaciones_dragon', cotizaciones); document.getElementById('cotizaciones').innerText = cotizaciones; window.open(`https://wa.me/527779107055?text=Me%20interesa%20el%20paquete%20de%20${pack}`, '_blank'); };
    </script>
</body>
</html>