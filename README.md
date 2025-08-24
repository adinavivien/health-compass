# health-compass

<!DOCTYPE html>
<html lang="de">
<head>
  <meta charset="UTF-8">
  <title>Mandelbutter – Health Compass</title>
  <style>
    body {
      font-family: Arial, sans-serif;
      background: #f9f9f9;
      display: flex;
      flex-direction: column;
      align-items: center;
      justify-content: flex-start;
      min-height: 100vh;
      margin: 0;
      padding: 20px;
    }
    h1 {
      margin-bottom: 20px;
    }
    .compass {
      position: relative;
      width: 400px;
      height: 400px;
      margin-bottom: 30px;
    }
    .smiley {
      position: absolute;
      top: 50%;
      left: 50%;
      transform: translate(-50%, -50%);
      font-size: 80px;
      color: green; /* Smiley grün einfärben */
    }
    .box {
      position: absolute;
      width: 120px;
      height: 60px;
      display: flex;
      align-items: center;
      justify-content: center;
      font-weight: bold;
      color: white;
      border-radius: 8px;
      text-align: center;
      padding: 5px;
    }
    /* Box-Positionen */
    .fett { top: 0; left: 50%; transform: translateX(-50%); background: red; }
    .zucker { top: 50%; left: 0; transform: translateY(-50%); background: green; }
    .salz { bottom: 0; left: 50%; transform: translateX(-50%); background: green; }
    .co2 { top: 50%; right: 0; transform: translateY(-50%); background: gold; color: black; }
    .processing { top: 10%; right: 10%; background: green; }
    /* Legende */
    .legende {
      background: white;
      border: 1px solid #ccc;
      border-radius: 8px;
      padding: 15px;
      max-width: 400px;
      font-size: 14px;
      line-height: 1.6;
    }
    .legend-item {
      display: flex;
      align-items: center;
      margin-bottom: 5px;
    }
    .legend-color {
      width: 20px;
      height: 20px;
      border-radius: 4px;
      margin-right: 8px;
    }
  </style>
</head>
<body>
  <h1>Mandelbutter</h1>
  <div class="compass">
    <!-- Grüner Smiley -->
    <div class="smiley">🙂</div>
    <!-- Boxen -->
    <div class="box fett">Fett: 55g (rot)</div>
    <div class="box zucker">Zucker: 4g (grün)</div>
    <div class="box salz">Salz: 0,02g (grün)</div>
    <div class="box co2">CO₂: 2,5kg (gelb)</div>
    <div class="box processing">Processing: 2 (grün)</div>
  </div>
  <!-- Legende -->
  <div class="legende">
    <div class="legend-item"><div class="legend-color" style="background:red;"></div> Rot = hoch / ungünstig</div>
    <div class="legend-item"><div class="legend-color" style="background:green;"></div> Grün = niedrig / günstig</div>
    <div class="legend-item"><div class="legend-color" style="background:gold;"></div> Gelb = mittel</div>
    <div class="legend-item">🙂 = insgesamt positiv</div>
    <div class="legend-item">😐 = mittel</div>
    <div class="legend-item">🙁 = negativ</div>
  </div>
</body>
</html>
