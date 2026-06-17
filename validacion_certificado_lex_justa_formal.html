<!DOCTYPE html>
<html lang="es">
<head>
  <meta charset="UTF-8" />
  <meta name="viewport" content="width=device-width, initial-scale=1.0" />
  <title>Validación de Certificado | Lex Justa</title>
  <style>
    :root {
      --navy: #0f2348;
      --gold: #b58a2f;
      --gold-soft: #d3b36a;
      --bg: #f4f6fa;
      --text: #1f2430;
      --muted: #5d6778;
      --border: #d9dee8;
      --valid-bg: #edf8f0;
      --valid-border: #4a9c65;
      --invalid-bg: #fff3f1;
      --invalid-border: #b5534c;
      --shadow: 0 18px 45px rgba(12, 24, 49, 0.12);
    }

    * { box-sizing: border-box; }

    body {
      margin: 0;
      font-family: "Georgia", "Times New Roman", serif;
      background: linear-gradient(180deg, #eef2f8 0%, #f7f8fb 100%);
      color: var(--text);
    }

    .topbar {
      height: 8px;
      background: linear-gradient(90deg, var(--gold) 0%, var(--navy) 55%, var(--gold) 100%);
    }

    .page {
      min-height: calc(100vh - 8px);
      display: flex;
      align-items: center;
      justify-content: center;
      padding: 34px 18px;
    }

    .card {
      width: 100%;
      max-width: 930px;
      background: #fff;
      border: 1px solid #e6e9f0;
      border-radius: 18px;
      box-shadow: var(--shadow);
      overflow: hidden;
    }

    .header {
      padding: 34px 34px 24px;
      border-bottom: 1px solid #edf0f5;
      background:
        radial-gradient(circle at top right, rgba(181,138,47,0.10), transparent 28%),
        linear-gradient(180deg, #ffffff 0%, #fbfcfe 100%);
      text-align: center;
    }

    .seal {
      width: 76px;
      height: 76px;
      margin: 0 auto 14px;
      border-radius: 50%;
      border: 3px solid var(--gold);
      display: flex;
      align-items: center;
      justify-content: center;
      color: var(--navy);
      font-size: 31px;
      line-height: 1;
      background: radial-gradient(circle at 30% 30%, #fff8e8 0%, #f5e3b4 45%, #ecd39b 100%);
      box-shadow: inset 0 0 0 3px rgba(255,255,255,0.65);
    }

    .org {
      font-size: 15px;
      letter-spacing: 1.7px;
      text-transform: uppercase;
      color: var(--navy);
      font-weight: 700;
      margin-bottom: 8px;
    }

    h1 {
      margin: 0;
      color: var(--navy);
      font-size: clamp(28px, 4vw, 42px);
      letter-spacing: 1px;
      font-weight: 700;
    }

    .subtitle {
      margin-top: 10px;
      color: var(--muted);
      font-size: 16px;
      line-height: 1.6;
    }

    .content {
      padding: 30px 34px 34px;
      display: grid;
      grid-template-columns: 1.05fr 0.95fr;
      gap: 28px;
    }

    .panel {
      border: 1px solid var(--border);
      border-radius: 16px;
      padding: 24px;
      background: #fff;
    }

    .panel h2 {
      margin: 0 0 14px;
      color: var(--navy);
      font-size: 22px;
      font-weight: 700;
    }

    .panel p, .panel li {
      color: var(--muted);
      font-size: 15px;
      line-height: 1.65;
      margin: 0;
    }

    .instructions {
      padding-left: 18px;
      margin: 0;
    }

    .instructions li + li { margin-top: 10px; }

    .label {
      display: block;
      font-size: 14px;
      color: var(--navy);
      margin-bottom: 10px;
      font-weight: 700;
      letter-spacing: 0.2px;
    }

    .input-row {
      display: flex;
      gap: 12px;
      flex-wrap: wrap;
    }

    input[type="text"] {
      flex: 1 1 280px;
      min-width: 0;
      padding: 15px 16px;
      border-radius: 12px;
      border: 1px solid #cfd6e2;
      font-size: 16px;
      font-family: Arial, Helvetica, sans-serif;
      color: #132238;
      outline: none;
      transition: border-color .2s ease, box-shadow .2s ease;
      text-transform: uppercase;
    }

    input[type="text"]:focus {
      border-color: var(--navy);
      box-shadow: 0 0 0 4px rgba(15,35,72,0.08);
    }

    button {
      padding: 14px 24px;
      border: none;
      border-radius: 12px;
      background: linear-gradient(180deg, #15315f 0%, #0f2348 100%);
      color: #fff;
      font-size: 15px;
      font-weight: 700;
      letter-spacing: 0.3px;
      cursor: pointer;
      min-width: 154px;
      box-shadow: 0 10px 22px rgba(15,35,72,0.18);
    }

    button:hover { filter: brightness(1.03); }

    .helper {
      margin-top: 12px;
      font-size: 13px;
      color: #6e7889;
      font-family: Arial, Helvetica, sans-serif;
    }

    .result {
      margin-top: 22px;
      display: none;
      border-radius: 14px;
      padding: 18px;
      font-family: Arial, Helvetica, sans-serif;
    }

    .result.show { display: block; }

    .result.valid {
      background: var(--valid-bg);
      border: 1px solid var(--valid-border);
    }

    .result.invalid {
      background: var(--invalid-bg);
      border: 1px solid var(--invalid-border);
    }

    .status {
      font-size: 18px;
      font-weight: 700;
      margin-bottom: 10px;
      color: #16311f;
    }

    .invalid .status { color: #6c1f1a; }

    .details {
      display: grid;
      grid-template-columns: 1fr;
      gap: 10px;
      margin-top: 12px;
    }

    .detail-item {
      display: grid;
      grid-template-columns: 170px 1fr;
      gap: 10px;
      padding-bottom: 8px;
      border-bottom: 1px dashed rgba(15,35,72,0.12);
    }

    .detail-item:last-child {
      border-bottom: none;
      padding-bottom: 0;
    }

    .detail-label {
      color: #354156;
      font-weight: 700;
    }

    .detail-value {
      color: #1b2432;
    }

    .footer {
      padding: 0 34px 30px;
      display: flex;
      justify-content: space-between;
      gap: 16px;
      flex-wrap: wrap;
      color: #677082;
      font-size: 13px;
      font-family: Arial, Helvetica, sans-serif;
    }

    .footer a {
      color: var(--navy);
      text-decoration: none;
      font-weight: 700;
    }

    @media (max-width: 760px) {
      .content {
        grid-template-columns: 1fr;
        padding: 24px 18px;
      }
      .header { padding: 28px 20px 20px; }
      .panel { padding: 20px; }
      .footer { padding: 0 18px 24px; }
      .detail-item { grid-template-columns: 1fr; gap: 4px; }
      button { width: 100%; }
    }
  </style>
</head>
<body>
  <div class="topbar"></div>
  <div class="page">
    <main class="card">
      <section class="header">
        <div class="seal">⚖</div>
        <div class="org">Lex Justa - Asociación Jurídica</div>
        <h1>Validación de Certificados</h1>
        <p class="subtitle">
          Plataforma de consulta para verificar la autenticidad de certificados emitidos por la institución.
        </p>
      </section>

      <section class="content">
        <article class="panel">
          <h2>Consulta de autenticidad</h2>
          <label class="label" for="codigo">Ingrese el código del certificado</label>
          <div class="input-row">
            <input id="codigo" type="text" placeholder="Ejemplo: CERT-2026-001" autocomplete="off" />
            <button type="button" onclick="validarCertificado()">Validar código</button>
          </div>
          <div class="helper">Solo los certificados registrados mostrarán información oficial de verificación.</div>

          <div id="resultado" class="result" aria-live="polite"></div>
        </article>

        <aside class="panel">
          <h2>Indicaciones</h2>
          <ol class="instructions">
            <li>Escriba el código completo del certificado en el campo de validación.</li>
            <li>Seleccione el botón <strong>“Validar código”</strong> para iniciar la consulta.</li>
            <li>Si el código es auténtico y está registrado, el sistema mostrará los datos del titular.</li>
            <li>Si el código no existe o no corresponde al registro, el resultado aparecerá como <strong>inválido</strong>.</li>
          </ol>
        </aside>
      </section>

      <div class="footer">
        <div>Registro institucional de verificación documental.</div>
        <div>Página oficial: <a href="https://www.facebook.com/share/1GmrUH5KiE/" target="_blank" rel="noopener noreferrer">Lex Justa - Facebook</a></div>
      </div>
    </main>
  </div>

  <script>
    const certificadoRegistrado = {
      codigo: 'CERT-2026-001',
      numeroCertificado: '126-2025',
      titular: 'Yorvin Bruce Saldaña Ocmin',
      dni: '75879142',
      curso: 'Ley de Procedimiento Administrativo General - Ley N.º 27444; Derecho Administrativo & Derecho Constitucional',
      condicion: 'Asistente',
      horas: '90 horas académicas',
      nota: 'Dieciocho (18)',
      fechas: 'Del sábado 04 de octubre de 2025 al domingo 02 de noviembre de 2025',
      emision: '15 de noviembre de 2025',
      institucion: 'Lex Justa - Asociación Jurídica'
    };

    function escapeHtml(texto) {
      return texto
        .replace(/&/g, '&amp;')
        .replace(/</g, '&lt;')
        .replace(/>/g, '&gt;')
        .replace(/"/g, '&quot;')
        .replace(/'/g, '&#039;');
    }

    function validarCertificado() {
      const input = document.getElementById('codigo');
      const resultado = document.getElementById('resultado');
      const codigoIngresado = input.value.trim().toUpperCase();
      const codigoValido = certificadoRegistrado.codigo.toUpperCase();

      if (!codigoIngresado) {
        resultado.className = 'result show invalid';
        resultado.innerHTML = `
          <div class="status">Resultado: código inválido</div>
          <div>Por favor, ingrese un código de certificado para realizar la validación.</div>
        `;
        return;
      }

      if (codigoIngresado === codigoValido) {
        resultado.className = 'result show valid';
        resultado.innerHTML = `
          <div class="status">Resultado: certificado válido</div>
          <div>El código consultado se encuentra registrado en el sistema.</div>
          <div class="details">
            <div class="detail-item"><div class="detail-label">Código</div><div class="detail-value">${escapeHtml(certificadoRegistrado.codigo)}</div></div>
            <div class="detail-item"><div class="detail-label">N.º de certificado</div><div class="detail-value">${escapeHtml(certificadoRegistrado.numeroCertificado)}</div></div>
            <div class="detail-item"><div class="detail-label">Titular</div><div class="detail-value">${escapeHtml(certificadoRegistrado.titular)}</div></div>
            <div class="detail-item"><div class="detail-label">DNI</div><div class="detail-value">${escapeHtml(certificadoRegistrado.dni)}</div></div>
            <div class="detail-item"><div class="detail-label">Programa</div><div class="detail-value">${escapeHtml(certificadoRegistrado.curso)}</div></div>
            <div class="detail-item"><div class="detail-label">Condición</div><div class="detail-value">${escapeHtml(certificadoRegistrado.condicion)}</div></div>
            <div class="detail-item"><div class="detail-label">Duración</div><div class="detail-value">${escapeHtml(certificadoRegistrado.horas)}</div></div>
            <div class="detail-item"><div class="detail-label">Calificación</div><div class="detail-value">${escapeHtml(certificadoRegistrado.nota)}</div></div>
            <div class="detail-item"><div class="detail-label">Fechas del evento</div><div class="detail-value">${escapeHtml(certificadoRegistrado.fechas)}</div></div>
            <div class="detail-item"><div class="detail-label">Fecha de emisión</div><div class="detail-value">${escapeHtml(certificadoRegistrado.emision)}</div></div>
            <div class="detail-item"><div class="detail-label">Institución emisora</div><div class="detail-value">${escapeHtml(certificadoRegistrado.institucion)}</div></div>
          </div>
        `;
      } else {
        resultado.className = 'result show invalid';
        resultado.innerHTML = `
          <div class="status">Resultado: certificado inválido</div>
          <div>El código ingresado no corresponde a ningún certificado registrado en esta plataforma.</div>
        `;
      }
    }

    document.getElementById('codigo').addEventListener('keydown', function(event) {
      if (event.key === 'Enter') {
        validarCertificado();
      }
    });
  </script>
</body>
</html>
