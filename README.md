<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>JS Master Style - Agendar Citas</title>
    <style>
        body {
            font-family: Arial, sans-serif;
            margin: 0;
            padding: 0;
            background-color: #f9f9f9;
        }
        header {
            background-color: #333;
            color: #fff;
            padding: 20px;
            text-align: center;
        }
        .container {
            max-width: 600px;
            margin: 20px auto;
            padding: 20px;
            background-color: #fff;
            border-radius: 8px;
            box-shadow: 0 2px 10px rgba(0, 0, 0, 0.1);
        }
        h1 {
            text-align: center;
        }
        form {
            display: flex;
            flex-direction: column;
        }
        label {
            margin-bottom: 5px;
            font-weight: bold;
        }
        input, select, button {
            margin-bottom: 15px;
            padding: 10px;
            border: 1px solid #ccc;
            border-radius: 5px;
        }
        button {
            background-color: #333;
            color: white;
            font-size: 16px;
            cursor: pointer;
        }
        button:hover {
            background-color: #555;
        }
    </style>
</head>
<body>
    <header>
        <h1>JS Master Style</h1>
        <p>Agende su cita con nosotros</p>
    </header>
    <div class="container">
        <h1>Agendar Cita</h1>
        <form action="/submit" method="POST">
            <label for="name">Nombre completo:</label>
            <input type="text" id="name" name="name" placeholder="Escribe tu nombre" required>

            <label for="phone">Teléfono:</label>
            <input type="tel" id="phone" name="phone" placeholder="Escribe tu número" required>

            <label for="date">Fecha:</label>
            <input type="date" id="date" name="date" required>

            <label for="time">Hora:</label>
            <input type="time" id="time" name="time" required>

            <label for="service">Servicio:</label>
            <select id="service" name="service" required>
                <option value="">Seleccione un servicio</option>
                <option value="corte">Corte de cabello</option>
                <option value="barba">Arreglo de barba</option>
                <option value="paquete">Corte y barba</option>
            </select>

            <button type="submit">Agendar</button>
        </form>
    </div>
</body>
</html>

