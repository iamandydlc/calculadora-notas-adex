<!-- Logo ADEX -->
<img 
  src="1781661864344.png" 
  alt="Logo ADEX Escuela" 
  class="logo"
>
>
<!DOCTYPE html>
<html lang="es">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Unidad Didáctica - Creatividad e Innovación | ADEX</title>
    <style>
        * {
            margin: 0;
            padding: 0;
            box-sizing: border-box;
            font-family: 'Segoe UI', Roboto, sans-serif;
        }

        body {
            background: linear-gradient(135deg, #003399 0%, #0055cc 100%);
            min-height: 100vh;
            padding: 2rem 1rem;
        }

        .encabezado {
            text-align: center;
            margin-bottom: 2rem;
            color: white;
        }

        .logo-adex {
            max-width: 220px;
            height: auto;
            margin-bottom: 1rem;
            filter: drop-shadow(0 2px 6px rgba(0,0,0,0.2));
        }

        .grupo-info {
            background: rgba(255,255,255,0.15);
            padding: 1.5rem;
            border-radius: 12px;
            margin: 1.5rem auto;
            max-width: 500px;
            border: 1px solid rgba(255,255,255,0.3);
        }

        .grupo-info h3 {
            margin-bottom: 1rem;
            font-size: 1.3rem;
        }

        .grupo-info ul {
            list-style: none;
            font-size: 1rem;
            line-height: 1.8;
        }

        h1 {
            font-size: 2rem;
            text-shadow: 2px 2px 4px rgba(0,0,0,0.2);
            margin-bottom: 0.8rem;
        }

        .contenedor-principal {
            max-width: 780px;
            margin: 0 auto;
            display: flex;
            flex-direction: column;
            gap: 1.8rem;
        }

        .tarjeta {
            background: #ffffff;
            padding: 1.8rem;
            border-radius: 16px;
            box-shadow: 0 8px 20px rgba(0,0,0,0.15);
        }

        h2 {
            color: #003399;
            margin-bottom: 1.2rem;
            font-size: 1.4rem;
            border-bottom: 2px solid #0055cc;
            padding-bottom: 0.5rem;
        }

        .datos-generales {
            display: grid;
            gap: 1rem;
            font-size: 1rem;
        }

        .dato {
            display: flex;
            justify-content: space-between;
            padding: 0.8rem 1rem;
            background: #f0f5ff;
            border-radius: 8px;
            border-left: 4px solid #0055cc;
        }

        .etiqueta {
            font-weight: 600;
            color: #003399;
        }

        table {
            width: 100%;
            border-collapse: collapse;
            margin-top: 1rem;
            font-size: 0.95rem;
        }

        th, td {
            padding: 0.8rem;
            text-align: left;
            border-bottom: 1px solid #e0e7ff;
        }

        th {
            background-color: #003399;
            color: white;
        }

        tr:nth-child(even) {
            background-color: #f8fbff;
        }

        .leyenda {
            margin-top: 1rem;
            font-size: 0.9rem;
            display: grid;
            grid-template-columns: auto 1fr;
            gap: 0.4rem 0.8rem;
            align-items: center;
        }

        .color {
            width: 16px;
            height: 16px;
            display: inline-block;
            border-radius: 3px;
        }

        .configuracion {
            display: flex;
            gap: 1.2rem;
            margin-bottom: 1.5rem;
            flex-wrap: wrap;
            background: #f0f7ff;
            padding: 1rem;
            border-radius: 10px;
        }

        .campo {
            flex: 1;
            min-width: 180px;
        }

        label {
            display: block;
            font-weight: 600;
            margin-bottom: 0.5rem;
            color: #2d3748;
        }

        input {
            width: 100%;
            padding: 0.75rem;
            border: 2px solid #cbd5e1;
            border-radius: 8px;
            font-size: 1rem;
            transition: all 0.2s;
        }

        input:focus {
            outline: none;
            border-color: #0055cc;
            box-shadow: 0 0 0 3px rgba(0, 85, 204, 0.2);
        }

        .fila-nota {
            display: flex;
            gap: 1rem;
            margin-bottom: 1rem;
            align-items: center;
            flex-wrap: wrap;
            background: #f8fbff;
            padding: 1rem;
            border-radius: 10px;
            border-left: 4px solid #0055cc;
        }

        button {
            padding: 0.8rem 1.2rem;
            border: none;
            border-radius: 8px;
            font-weight: 600;
            cursor: pointer;
            transition: all 0.2s;
            box-shadow: 0 2px 6px rgba(0,0,0,0.1);
        }

        .btn-agregar {
            background: linear-gradient(90deg, #0099cc, #0055cc);
            color: white;
            margin-bottom: 1.5rem;
        }

        .btn-calcular {
            background: linear-gradient(90deg, #38a169, #2f855a);
            color: white;
            margin-right: 0.8rem;
        }

        .btn-limpiar {
            background: linear-gradient(90deg, #e53e3e, #c53030);
            color: white;
        }

        .btn-eliminar {
            background: linear-gradient(90deg, #ed8936, #dd6b20);
            color: white;
            padding: 0.5rem 0.9rem;
        }

        button:hover {
            transform: translateY(-2px);
            box-shadow: 0 4px 10px rgba(0,0,0,0.15);
        }

        .resultado {
            margin-top: 1.8rem;
            padding: 1.5rem;
            border-radius: 12px;
            font-size: 1.2rem;
            font-weight: 600;
            text-align: center;
            display: none;
        }

        .aprobado {
            background: linear-gradient(135deg, #48bb78, #2f855a);
            color: white;
        }

        .reprobado {
            background: linear-gradient(135deg, #f56565, #c53030);
            color: white;
        }
    </style>
</head>
<body>

    <div class="encabezado">
        <img src="https://www.adexperu.org.pe/wp-content/uploads/2020/07/logo-adex.png" alt="Logo ADEX Escuela" class="logo-adex">
        <h1>Creatividad e Innovación</h1>
        <p>Unidad Didáctica | ADEX Escuela de Especialización</p>

        <div class="grupo-info">
            <h3>📚 Grupo 3</h3>
            <ul>
                <li>Jhon Dayron Zárate</li>
                <li>Joel Hualpa</li>
                <li>Luis Yaranga</li>
                <li>Orlando Zacarías</li>
                <li>Matías Martinez</li>
                <li>Andi De la Cruz</li>
                <li>Fatima</li>
            </ul>
        </div>
    </div>

    <div class="contenedor-principal">

        <div class="tarjeta">
            <h2>📋 Datos Generales de la Unidad Didáctica</h2>
            <div class="datos-generales">
                <div class="dato">
                    <span class="etiqueta">Tipo de UD:</span>
                    <span>Transversal para la línea de investigación</span>
                </div>
                <div class="dato">
                    <span class="etiqueta">Actividades y evidencias:</span>
                    <span>3 actividades de aprendizaje y 3 evidencias</span>
                </div>
                <div class="dato">
                    <span class="etiqueta">Créditos y duración:</span>
                    <span>4 créditos | 80 horas totales</span>
                </div>
                <div class="dato">
                    <span class="etiqueta">Sesiones:</span>
                    <span>14 sesiones de 4.71 horas académicas (257 min) cada una</span>
                </div>
            </div>
        </div>

        <div class="tarjeta">
            <h2>📅 Estructura de la Unidad Didáctica</h2>
            <table>
                <thead>
                    <tr>
                        <th>Semana</th>
                        <th>Actividad / Sesión</th>
                    </tr>
                </thead>
                <tbody>
                    <tr><td>1</td><td>Sesión 1 (Foro) - Evaluación diagnóstica</td></tr>
                    <tr><td>2</td><td>Sesión 2 (Participación activa)</td></tr>
                    <tr><td>3</td><td>Sesión 3 (Participación activa)</td></tr>
                    <tr><td>4</td><td>Sesión 4 (Participación activa)</td></tr>
                    <tr><td>5</td><td>Sesión 5 (Cuestionario)</td></tr>
                    <tr><td>6</td><td>Sesión 6 - Act. CE - Evidencia evaluativa 1</td></tr>
                    <tr><td>7</td><td>Sesión 7 (Foro)</td></tr>
                    <tr><td>8</td><td>Sesión 8 (Participación activa)</td></tr>
                    <tr><td>9</td><td>Sesión 9 (Cuestionario)</td></tr>
                    <tr><td>10</td><td>Sesión 10 - Act. CE - Evidencia evaluativa 2</td></tr>
                    <tr><td>11</td><td>Sesión 11 (Foro)</td></tr>
                    <tr><td>12</td><td>Sesión 12 (Participación activa)</td></tr>
                    <tr><td>13</td><td>Sesión 13 (Cuestionario) - Act. CE</td></tr>
                    <tr><td>14</td><td>Sesión 14 - Evidencia evaluativa 3</td></tr>
                </tbody>
            </table>

            <div class="leyenda">
                <span><span class="color" style="background:#000000"></span></span>
                <span>Recursos para desarrollo de sesión</span>
                <span><span class="color" style="background:#1a365d"></span></span>
                <span>Evaluaciones grupales</span>
                <span><span class="color" style="background:#92400e"></span></span>
                <span>Evaluaciones individuales</span>
                <span><span class="color" style="background:#7e22ce"></span></span>
                <span>Actividades para empleabilidad (CE)</span>
            </div>
        </div>

        <div class="tarjeta">
            <h2>📊 Sistema de Evaluación</h2>
            <p style="margin-bottom:1rem; color:#4a5568;">Evaluación continua dividida en 3 evidencias:</p>

            <table>
                <thead>
                    <tr>
                        <th>Sesión</th>
                        <th>Evaluación</th>
                        <th>Peso (%)</th>
                    </tr>
                </thead>
                <tbody>
                    <tr><td>6</td><td>EC1</td><td>20%</td></tr>
                    <tr><td>10</td><td>EC2</td><td>35%</td></tr>
                    <tr><td>14</td><td>EC3</td><td>45%</td></tr>
                </tbody>
            </table>

            <h3 style="margin-top:1.2rem; color:#003399; font-size:1.1rem;">Cada evidencia se compone de:</h3>
            <table>
                <thead>
                    <tr>
                        <th>Actividad</th>
                        <th>Peso (%)</th>
                    </tr>
                </thead>
                <tbody>
                    <tr><td>Foro (coevaluación)</td><td>10%</td></tr>
                    <tr><td>Participación activa</td><td>20%</td></tr>
                    <tr><td>Cuestionario</td><td>20%</td></tr>
                    <tr><td>Evidencia evaluativa</td><td>50%</td></tr>
                </tbody>
            </table>
            <p style="margin-top:0.8rem; font-size:0.9rem; color:#4a5568; font-style:italic;">* Incluye además intervenciones orales, trabajo en equipo, responsabilidad y comunicación.</p>
        </div>

        <div class="tarjeta">
            <h2>🧮 Calculadora de Notas</h2>

            <div class="configuracion">
                <div class="campo">
                    <label>Nota mínima para aprobar</label>
                    <input type="number" id="notaAprobacion" value="11" min="0" max="20" step="0.1">
                </div>
                <div class="campo">
                    <label>Nota máxima</label>
                    <input type="number" id="notaMaxima" value="20" min="1" max="100">
                </div>
            </div>

            <div id="contenedorNotas"></div>

            <button class="btn-agregar" onclick="agregarFila()">+ Agregar nota</button>
            <br><br>
            <button class="btn-calcular" onclick="calcularPromedio()">📊 Calcular Promedio</button>
            <button class="btn-limpiar" onclick="limpiarTodo()">🔄 Reiniciar</button>

            <div id="cajaResultado" class="resultado"></div>
        </div>

    </div>

    <script>
        function agregarFila() {
            const contenedor = document.getElementById('contenedorNotas');
            const notaMax = document.getElementById('notaMaxima').value;
            const fila = document.createElement('div');
            fila.className = 'fila-nota';
            fila.innerHTML = `
                <div class="campo">
                    <label>Nota obtenida</label>
                    <input type="number" class="nota" min="0" max="${notaMax}" step="0.1" placeholder="Ej: 15">
                </div>
                <div class="campo">
                    <label>Ponderación (%)</label>
                    <input type="number" class="peso" min="0" max="100" step="0.1" placeholder="Ej: 20">
                </div>
                <button class="btn-eliminar" onclick="eliminarFila(this)">×</button>
            `;
            contenedor.appendChild(fila);
        }

        function eliminarFila(boton) {
            boton.parentElement.remove();
        }

        function calcularPromedio() {
            const notas = document.querySelectorAll('.nota');
            const pesos = document.querySelectorAll('.peso');
            const notaMin = parseFloat(document.getElementById('notaAprobacion').value);
            const notaMax = parseFloat(document.getElementById('notaMaxima').value);
            let sumaPonderada = 0;
            let sumaPesos = 0;

            for (let i = 0; i < notas.length; i++) {
                const n = parseFloat(notas[i].value);
                const p = parseFloat(pesos[i].value);
                if (isNaN(n) || isNaN(p) || n < 0 || n > notaMax || p < 0 || p > 100) {
                    alert('Ingresa valores válidos entre 0 y ' + notaMax);
                    return;
                }
                sumaPonderada += n * p;
                sumaPesos += p;
            }

            if (sumaPesos === 0 || sumaPesos > 100) {
                alert('La suma de porcentajes debe ser mayor a 0 y menor o igual a 100%');
                return;
            }

            const promedio = sumaPonderada / sumaPesos;
            const resultado = document.getElementById('cajaResultado');
            resultado.style.display = 'block';

            if (promedio >= notaMin) {
                resultado.className = 'resultado aprobado';
                resultado.innerHTML = `✅ Promedio final: ${promedio.toFixed(2)}<br>¡APROBADO!`;
            } else {
                resultado.className = 'resultado reprobado';
                resultado.innerHTML = `❌ Promedio final: ${promedio.toFixed(2)}<br>REPROBADO`;
            }
        }

        function limpiarTodo() {
            document.getElementById('contenedorNotas').innerHTML = '';
            document.getElementById('cajaResultado').style.display = 'none';
            agregarFila();
        }

        window.onload = agregarFila;
    </script>

</body>
</html>
