from pathlib import Path
# Crear una versión formal con el código 126-2025 y logo incrustado.
# Usaremos como logo el emblema disponible dentro del certificado adjunto, recortándolo del certificado original.

from PIL import Image
import base64, io, os, textwrap

cert_path = Path("/mnt/data/20369.jpg")
img = Image.open(cert_path).convert("RGBA")

# Recorte aproximado del logo circular en la esquina superior izquierda del certificado nuevo.
# Coordenadas basadas en la imagen adjunta del certificado.
logo_crop = img.crop((70, 45, 385, 365))
logo_path = Path("/mnt/data/logo_lex_justa.png")
logo_crop.save(logo_path)

# Convertir logo a base64 para que GitHub Pages no dependa de archivos aparte.
with open(logo_path, "rb") as f:
    logo_b64 = base64.b64encode(f.read()).decode("utf-8")

html = f"""<!DOCTYPE html>
<html lang="es">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <title>Validación de Certificado | Lex Justa</title>
  <style>
    :root {{
      --azul: #0b1f44;
      --azul2: #132f63;
      --dorado: #b8892f;
      --dorado2: #d4b36a;
      --fondo: #f3f5f9;
      --texto: #1f2633;
      --gris: #667085;
      --borde: #d9dee8;
      --verde: #1f7a3f;
      --rojo: #9b2c25;
    }}

    * {{
      box-sizing: border-box;
    }}

    body {{
      margin: 0;
      font-family: Arial, Helvetica, sans-serif;
      background: linear-gradient(180deg, #eef2f7 0%, #f8f9fc 100%);
      color: var(--texto);
    }}

    .barra {{
      height: 9px;
      background: linear-gradient(90deg, var(--dorado), var(--azul), var(--dorado));
    }}

    .contenedor {{
      min-height: calc(100vh - 9px);
      display: flex;
      align-items: center;
      justify-content: center;
      padding: 32px 16px;
    }}

    .tarjeta {{
      width: 100%;
      max-width: 980px;
      background: #ffffff;
      border: 1px solid #e4e7ef;
      border-radius: 18px;
      box-shadow: 0 18px 45px rgba(10, 24, 50, 0.14);
      overflow: hidden;
    }}

    .encabezado {{
      text-align: center;
      padding: 34px 28px 26px;
      background:
        radial-gradient(circle at top right, rgba(184, 137, 47, 0.12), transparent 30%),
        linear-gradient(180deg, #ffffff 0%, #fbfcff 100%);
      border-bottom: 1px solid #e9edf5;
    }}

    .logo {{
      width: 108px;
      height: 108px;
      object-fit: contain;
      margin: 0 auto 14px;
      display: block;
      border-radius: 50%;
      filter: drop-shadow(0 8px 12px rgba(11, 31, 68, 0.15));
    }}

    .institucion {{
      color: var(--azul);
      font-weight: 700;
      text-transform: uppercase;
      letter-spacing: 1.6px;
      font-size: 15px;
      margin-bottom: 8px;
    }}

    h1 {{
      margin: 0;
      color: var(--azul);
      font-family: Georgia, "Times New Roman", serif;
      font-size: clamp(30px, 4vw, 44px);
      letter-spacing: 0.6px;
    }}

    .subtitulo {{
      max-width: 760px;
      margin: 12px auto 0;
      color: var(--gris);
      line-height: 1.6;
      font-size: 16px;
    }}

    .contenido {{
      display: grid;
      grid-template-columns: 1.08fr 0.92fr;
      gap: 26px;
      padding: 30px;
    }}

    .panel {{
      border: 1px solid var(--borde);
      border-radius: 16px;
      padding: 24px;
      background: #ffffff;
    }}

    .panel h2 {{
      margin: 0 0 14px;
      color: var(--azul);
      font-size: 22px;
    }}

    .panel p,
    .panel li {{
      color: var(--gris);
      line-height: 1.65;
      font-size: 15px;
    }}

    label {{
      display: block;
      margin-bottom: 10px;
      color: var(--azul);
      font-weight: 700;
      font-size: 14px;
    }}

    .fila {{
      display: flex;
      gap: 12px;
      flex-wrap: wrap;
    }}

    input {{
      flex: 1 1 260px;
      padding: 15px 16px;
      border: 1px solid #cfd6e2;
      border-radius: 12px;
      font-size: 16px;
      outline: none;
      text-transform: uppercase;
    }}

    input:focus {{
      border-color: var(--azul);
      box-shadow: 0 0 0 4px rgba(11, 31, 68, 0.08);
    }}

    button {{
      min-width: 150px;
      border: none;
      border-radius: 12px;
      background: linear-gradient(180deg, var(--azul2), var(--azul));
      color: #ffffff;
      font-weight: 700;
      font-size: 15px;
      cursor: pointer;
      padding: 14px 22px;
      box-shadow: 0 10px 22px rgba(11, 31, 68, 0.18);
    }}

    button:hover {{
      filter: brightness(1.05);
    }}

    .nota {{
      margin-top: 12px;
      font-size: 13px;
      color: #6b7280;
    }}

    .resultado {{
      display: none;
      margin-top: 22px;
      border-radius: 14px;
      padding: 18px;
      line-height: 1.5;
    }}

    .resultado.mostrar {{
      display: block;
    }}

    .valido {{
      background: #eefaf2;
      border: 1px solid #62a877;
    }}

    .invalido {{
      background: #fff2f0;
      border: 1px solid #c46a62;
    }}

    .estado {{
      font-size: 18px;
      font-weight: 800;
      margin-bottom: 8px;
    }}

    .valido .estado {{
      color: var(--verde);
    }}

    .invalido .estado {{
      color: var(--rojo);
    }}

    .datos {{
      margin-top: 14px;
      display: grid;
      gap: 10px;
    }}

    .dato {{
      display: grid;
      grid-template-columns: 175px 1fr;
      gap: 10px;
      padding-bottom: 9px;
      border-bottom: 1px dashed rgba(11, 31, 68, 0.15);
    }}

    .dato:last-child {{
      border-bottom: none;
      padding-bottom: 0;
    }}

    .etiqueta {{
      font-weight: 700;
      color: #334155;
    }}

    .valor {{
      color: #111827;
    }}

    .lista {{
      margin: 0;
      padding-left: 20px;
    }}

    .pie {{
      padding: 0 30px 30px;
      color: #667085;
      font-size: 13px;
      display: flex;
      justify-content: space-between;
      gap: 14px;
      flex-wrap: wrap;
    }}

    .pie a {{
      color: var(--azul);
      font-weight: 700;
      text-decoration: none;
    }}

    @media (max-width: 760px) {{
      .contenido {{
        grid-template-columns: 1fr;
        padding: 22px 16px;
      }}

      .encabezado {{
        padding: 28px 18px 22px;
      }}

      .panel {{
        padding: 20px;
      }}

      .dato {{
        grid-template-columns: 1fr;
        gap: 4px;
      }}

      button {{
        width: 100%;
      }}

      .pie {{
        padding: 0 16px 24px;
      }}
    }}
  </style>
</head>
<body>
  <div class="barra"></div>

  <main class="contenedor">
    <section class="tarjeta">
      <header class="encabezado">
        <img class="logo" src="data:image/png;base64,{logo_b64}" alt="Logo de Lex Justa">
        <div class="institucion">Lex Justa - Asociación Jurídica</div>
        <h1>Validación de Certificados</h1>
        <p class="subtitulo">
          Sistema institucional de consulta para verificar la autenticidad de certificados emitidos por Lex Justa - Asociación Jurídica.
        </p>
      </header>

      <section class="contenido">
        <article class="panel">
          <h2>Consulta de autenticidad</h2>

          <label for="codigo">Ingrese el código del certificado</label>
          <div class="fila">
            <input id="codigo" type="text" placeholder="Ejemplo: 126-2025" autocomplete="off">
            <button type="button" onclick="validarCertificado()">Validar</button>
          </div>

          <div class="nota">
            Código autorizado para este certificado: <strong>126-2025</strong>.
          </div>

          <div id="resultado" class="resultado" aria-live="polite"></div>
        </article>

        <aside class="panel">
          <h2>Indicaciones</h2>
          <ol class="lista">
            <li>Ingrese el código completo del certificado.</li>
            <li>Presione el botón <strong>Validar</strong>.</li>
            <li>Si el certificado está registrado, se mostrarán los datos del titular y del programa académico.</li>
            <li>Si el código no corresponde al registro, el sistema mostrará el certificado como inválido.</li>
          </ol>
        </aside>
      </section>

      <footer class="pie">
        <span>Registro institucional de verificación documental.</span>
        <span>Página oficial: <a href="https://www.facebook.com/share/1GmrUH5KiE/" target="_blank" rel="noopener noreferrer">Lex Justa - Facebook</a></span>
      </footer>
    </section>
  </main>

  <script>
    const certificado = {{
      codigo: "126-2025",
      titular: "Yorvin Bruce Saldaña Ocmin",
      dni: "75879142",
      numeroCertificado: "126 del año 2025",
      institucion: "Lex Justa - Asociación Jurídica",
      programa: "Ley de Procedimiento Administrativo General - Ley N.° 27444; Derecho Administrativo & Derecho Constitucional",
      condicion: "Asistente",
      duracion: "90 horas académicas",
      nota: "Dieciocho (18)",
      fechaEvento: "Del sábado 04 de octubre de 2025 al domingo 02 de noviembre de 2025",
      fechaEmision: "15 de noviembre de 2025"
    }};

    function limpiarTexto(texto) {{
      return texto
        .replace(/&/g, "&amp;")
        .replace(/</g, "&lt;")
        .replace(/>/g, "&gt;")
        .replace(/"/g, "&quot;")
        .replace(/'/g, "&#039;");
    }}

    function validarCertificado() {{
      const entrada = document.getElementById("codigo").value.trim().toUpperCase();
      const resultado = document.getElementById("resultado");
      const codigoCorrecto = certificado.codigo.toUpperCase();

      if (entrada === "") {{
        resultado.className = "resultado mostrar invalido";
        resultado.innerHTML = `
          <div class="estado">Resultado: código no ingresado</div>
          <div>Ingrese un código de certificado para realizar la validación.</div>
        `;
        return;
      }}

      if (entrada === codigoCorrecto) {{
        resultado.className = "resultado mostrar valido";
        resultado.innerHTML = `
          <div class="estado">Resultado: certificado válido</div>
          <div>El código consultado se encuentra registrado en la base de validación institucional.</div>

          <div class="datos">
            <div class="dato"><div class="etiqueta">Código</div><div class="valor">${{limpiarTexto(certificado.codigo)}}</div></div>
            <div class="dato"><div class="etiqueta">N.° de certificado</div><div class="valor">${{limpiarTexto(certificado.numeroCertificado)}}</div></div>
            <div class="dato"><div class="etiqueta">Titular</div><div class="valor">${{limpiarTexto(certificado.titular)}}</div></div>
            <div class="dato"><div class="etiqueta">DNI</div><div class="valor">${{limpiarTexto(certificado.dni)}}</div></div>
            <div class="dato"><div class="etiqueta">Programa</div><div class="valor">${{limpiarTexto(certificado.programa)}}</div></div>
            <div class="dato"><div class="etiqueta">Condición</div><div class="valor">${{limpiarTexto(certificado.condicion)}}</div></div>
            <div class="dato"><div class="etiqueta">Duración</div><div class="valor">${{limpiarTexto(certificado.duracion)}}</div></div>
            <div class="dato"><div class="etiqueta">Calificación</div><div class="valor">${{limpiarTexto(certificado.nota)}}</div></div>
            <div class="dato"><div class="etiqueta">Fecha del evento</div><div class="valor">${{limpiarTexto(certificado.fechaEvento)}}</div></div>
            <div class="dato"><div class="etiqueta">Fecha de emisión</div><div class="valor">${{limpiarTexto(certificado.fechaEmision)}}</div></div>
            <div class="dato"><div class="etiqueta">Entidad emisora</div><div class="valor">${{limpiarTexto(certificado.institucion)}}</div></div>
          </div>
        `;
      }} else {{
        resultado.className = "resultado mostrar invalido";
        resultado.innerHTML = `
          <div class="estado">Resultado: certificado inválido</div>
          <div>El código ingresado no corresponde a un certificado registrado en esta plataforma.</div>
        `;
      }}
    }}

    document.getElementById("codigo").addEventListener("keydown", function(event) {{
      if (event.key === "Enter") {{
        validarCertificado();
      }}
    }});
  </script>
</body>
</html>
"""

out = Path("/mnt/data/index.html")
out.write_text(html, encoding="utf-8")

# También guardamos una copia con nombre descriptivo
copy = Path("/mnt/data/validacion_lex_justa_codigo_126_2025.html")
copy.write_text(html, encoding="utf-8")

print("Archivos creados:")
print(out)
print(copy)
print(logo_path)
