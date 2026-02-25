<!DOCTYPE html>
<html lang="es">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Dedicatorias Musicales Personalizadas</title>
    <style>
        /* Estilos Generales */
        body {
            font-family: 'Segoe UI', Tahoma, Geneva, Verdana, sans-serif;
            margin: 0;
            padding: 0;
            background: linear-gradient(135deg, #667eea 0%, #764ba2 100%);
            min-height: 100vh;
            display: flex;
            justify-content: center;
            align-items: center;
            color: #333;
        }

        .container {
            background-color: #fff;
            padding: 40px;
            border-radius: 15px;
            box-shadow: 0 10px 25px rgba(0,0,0,0.2);
            width: 90%;
            max-width: 500px;
            margin: 20px;
        }

        header {
            text-align: center;
            margin-bottom: 30px;
        }

        header h1 {
            color: #4a148c;
            margin-bottom: 10px;
            font-size: 24px;
        }

        header p {
            color: #666;
            font-size: 14px;
        }

        /* Estilos del Formulario */
        .form-group {
            margin-bottom: 20px;
        }

        label {
            display: block;
            margin-bottom: 8px;
            font-weight: 600;
            color: #444;
        }

        input, select, textarea {
            width: 100%;
            padding: 12px;
            border: 1px solid #ddd;
            border-radius: 8px;
            box-sizing: border-box; /* Para que el padding no afecte el ancho */
            font-size: 16px;
            transition: border-color 0.3s;
        }

        input:focus, select:focus, textarea:focus {
            outline: none;
            border-color: #764ba2;
        }

        textarea {
            resize: vertical;
            height: 100px;
        }

        /* Estilos del Botón */
        .btn-whatsapp {
            display: block;
            width: 100%;
            background-color: #25D366;
            color: white;
            padding: 15px;
            border: none;
            border-radius: 8px;
            font-size: 18px;
            font-weight: bold;
            cursor: pointer;
            text-align: center;
            text-decoration: none;
            transition: background-color 0.3s, transform 0.2s;
            display: flex;
            justify-content: center;
            align-items: center;
            gap: 10px;
        }

        .btn-whatsapp:hover {
            background-color: #128C7E;
            transform: translateY(-2px);
        }

        /* Icono de WhatsApp simple con CSS */
        .icon-whatsapp {
            width: 24px;
            height: 24px;
            background-color: white;
            -webkit-mask: url('https://upload.wikimedia.org/wikipedia/commons/6/6b/WhatsApp.svg') no-repeat center;
            mask: url('https://upload.wikimedia.org/wikipedia/commons/6/6b/WhatsApp.svg') no-repeat center;
            background-color: white; 
            /* Truco para que el svg se vea blanco sobre fondo verde sin cargar imagen */
        }

        /* Nota sobre el número */
        .footer-note {
            text-align: center;
            margin-top: 20px;
            font-size: 12px;
            color: #888;
        }
    </style>
</head>
<body>

    <div class="container">
        <header>
            <h1>🎵 Dedicatorias Musicales</h1>
            <p>¿Quieres dedicar una canción especial? ¡Escríbeme y la personalizo para ti!</p>
        </header>

        <form id="musicForm">
            <!-- Tu Nombre -->
            <div class="form-group">
                <label for="nombreCliente">Tu Nombre:</label>
                <input type="text" id="nombreCliente" placeholder="Ej: Juan Pérez" required>
            </div>

            <!-- Nombre de quien recibe -->
            <div class="form-group">
                <label for="nombreDestinatario">Dedicado a:</label>
                <input type="text" id="nombreDestinatario" placeholder="Ej: María, mi jefe, mi mascota..." required>
            </div>

            <!-- Ocasion -->
            <div class="form-group">
                <label for="ocasion">Ocasión:</label>
                <select id="ocasion">
                    <option value="Cumpleaños">Cumpleaños</option>
                    <option value="Aniversario">Aniversario</option>
                    <option value="Pedir Perdón">Pedir Perdón</option>
                    <option value="Dedica Normal">Dedica Normal</option>
                    <option value="Negocio/Publicidad">Para mi Negocio</option>
                    <option value="Otro">Otro</option>
                </select>
            </div>

            <!-- Canción -->
            <div class="form-group">
                <label for="cancion">Canción preferida (Opcional):</label>
                <input type="text" id="cancion" placeholder="Título - Artista">
            </div>

            <!-- Mensaje -->
            <div class="form-group">
                <label for="mensaje">Tu mensaje personalizado:</label>
                <textarea id="mensaje" placeholder="Escribe lo que quieres que diga la canción..." required></textarea>
            </div>

            <!-- Botón -->
            <button type="submit" class="btn-whatsapp">
                <span>📱 Enviar Solicitud por WhatsApp</span>
            </button>
        </form>

        <div class="footer-note">
            <p>Asegúrate de tener WhatsApp instalado.</p>
        </div>
    </div>

    <script>
        document.getElementById('musicForm').addEventListener('submit', function(e) {
            e.preventDefault(); // Evita que el formulario se envíe de forma tradicional

            // 1. Obtener los valores
            const nombreCliente = document.getElementById('nombreCliente').value;
            const nombreDestinatario = document.getElementById('nombreDestinatario').value;
            const ocasion = document.getElementById('ocasion').value;
            const cancion = document.getElementById('cancion').value;
            const mensaje = document.getElementById('mensaje').value;

            // 2. Construir el texto del mensaje
            let texto = `🎵 *Nueva Solicitud de Dedicatoria* 🎵\n\n`;
            texto += `*De:* ${nombreCliente}\n`;
            texto += `*Para:* ${nombreDestinatario}\n`;
            texto += `*Ocasión:* ${ocasion}\n`;
            if(cancion) {
                texto += `*Canción:* ${cancion}\n`;
            }
            texto += `*Mensaje:*\n${mensaje}`;

            // 3. IMPORTANTE: Cambia este número poniéndole el código de país.
            // Ejemplo: Si es España (34), pon 34698904. Si es Perú (51), pon 51123456789.
            // El número que me diste: 74698904 (Parece de Perú o España sin 0).
            // ASUMIRE PERÚ (+51) PARA EL EJEMPLO. CAMBIA ESTO SI ES NECESARIO.
            const numeroTelefono = "51123456789"; // <--- REEMPLAZA ESTO CON TU NÚMERO COMPLETO (Ej: 34698904)

            // 4. Crear la URL de WhatsApp
            const urlWhatsapp = `https://wa.me/${numeroTelefono}?text=${encodeURIComponent(texto)}`;

            // 5. Abrir en nueva pestaña
            window.open(urlWhatsapp, '_blank');
        });
    </script>
</body>
</html>
