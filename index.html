<!DOCTYPE html>
<html lang="id">
<head>
  <meta charset="UTF-8" />
  <meta name="viewport" content="width=device-width, initial-scale=1.0" />
  <title>2050</title>

  <style>
    * { margin:0; padding:0; box-sizing:border-box; }

    body {
      font-family: 'Courier New', monospace;
      background: #000;
      color: #0f0;
      min-height: 100vh;
      overflow: hidden;
    }

    /* ── MAINTENANCE ── */
    #maintenance {
      position: fixed;
      inset: 0;
      background: #0a0a0a;
      display: flex;
      justify-content: center;
      align-items: center;
      z-index: 9999;
      transition: opacity 1s ease-out;
    }

    .maintenanceBox {
      background: #111;
      padding: 50px 40px;
      border-radius: 16px;
      text-align: center;
      border: 1px solid #333;
      box-shadow: 0 20px 60px rgba(0,0,0,0.9);
      max-width: 90%;
    }

    .maintenanceBox h1 {
      font-size: 28px;
      margin-bottom: 20px;
      color: #ccc;
    }

    #countdown {
      margin-top: 12px;
      color: #0f0;
      font-size: 24px;
      font-weight: bold;
      text-shadow: 0 0 12px #0f0, 0 0 24px #0f0;
      min-height: 40px;
      transition: all 0.3s ease;
    }

    #countdown::after {
      content: '';
      animation: blink 1.2s infinite;
    }

    @keyframes blink {
      0%,100% { opacity: 0.4; }
      50%     { opacity: 1; }
    }

    /* ── MATRIX RAIN ── */
    canvas {
      position: fixed;
      top: 0; left: 0;
      z-index: 1;
    }

    .overlay-text {
      position: absolute;
      top: 50%;
      left: 50%;
      transform: translate(-50%, -50%);
      font-family: 'Courier New', monospace;
      color: #0f0;
      text-align: center;
      text-shadow: 0 0 20px #0f0, 0 0 40px #0f0;
      pointer-events: none;
      z-index: 10;
      white-space: nowrap;
    }

    .big-year {
      font-size: clamp(70px, 20vw, 180px);
      font-weight: bold;
      margin: 10px 0;
    }

    .small {
      font-size: clamp(20px, 5.5vw, 42px);
      opacity: 0.85;
      margin-top: 15px;
    }
  </style>
</head>
<body>

<!-- MAINTENANCE -->
<div id="maintenance">
  <div class="maintenanceBox">
    <h1>🔒 Masa Depan</h1>
    <div id="countdown">Menghitung waktu...</div>
  </div>
</div>

<!-- MATRIX RAIN + TEXT -->
<canvas id="c"></canvas>

<div class="overlay-text" id="matrixText">
  <div>Haii</div>
  <div class="big-year">2050</div>
  <div class="small">aku kholiddzz dari 2026</div>
</div>

<script>
// ── TARGET WAKTU (format: YYYY-MM-DD HH:mm:ss) ──
const selesaiMaintenance = "2050-01-12 20:30:00";

const targetTime = new Date(selesaiMaintenance).getTime();

// ── UPDATE COUNTDOWN LEBIH HALUS ──
function updateCountdown() {
  const now = Date.now();
  const diff = targetTime - now;

  if (diff <= 0) {
    document.getElementById("maintenance").style.opacity = "0";
    setTimeout(() => {
      document.getElementById("maintenance").style.display = "none";
    }, 1000);
    return;
  }

  const hari   = Math.floor(diff / 86400000);
  const jam    = Math.floor((diff % 86400000) / 3600000);
  const menit  = Math.floor((diff % 3600000) / 60000);
  const detik  = Math.floor((diff % 60000) / 1000);

  const parts = [];
  if (hari   > 0) parts.push(`${hari} hari`);
  if (jam    > 0 || parts.length > 0) parts.push(`${jam.toString().padStart(2,'0')} jam`);
  if (menit  > 0 || parts.length > 0) parts.push(`${menit.toString().padStart(2,'0')} menit`);
  parts.push(`${detik.toString().padStart(2,'0')} detik`);

  document.getElementById("countdown").textContent = "Terbuka dalam " + parts.join(" ");
}

// Update lebih sering biar terasa hidup (200ms)
setInterval(updateCountdown, 200);
updateCountdown(); // panggil langsung sekali

// ── MATRIX RAIN ──
const canvas = document.getElementById('c');
const ctx = canvas.getContext('2d');

function resizeCanvas() {
  canvas.height = window.innerHeight;
  canvas.width = window.innerWidth;
}
resizeCanvas();
window.addEventListener('resize', resizeCanvas);

const chars = '01アイウエオカキクケコサシスセソタチツテトナニヌネノハヒフヘホマミムメモヤユヨラリルレロワヲンabcdefghijklmnopqrstuvwxyzABCDEFGHIJKLMNOPQRSTUVWXYZ0123456789@#$%^&*';
const fontSize = 16;
let columns = Math.floor(canvas.width / fontSize);
let drops = Array(columns).fill(1);

function drawMatrix() {
  ctx.fillStyle = 'rgba(0,0,0,0.05)';
  ctx.fillRect(0, 0, canvas.width, canvas.height);

  ctx.fillStyle = '#0f0';
  ctx.font = fontSize + 'px monospace';

  for (let i = 0; i < drops.length; i++) {
    const text = chars.charAt(Math.floor(Math.random() * chars.length));
    const x = i * fontSize;
    const y = drops[i] * fontSize;

    ctx.fillText(text, x, y);

    if (y > canvas.height && Math.random() > 0.975) drops[i] = 0;
    drops[i]++;
  }
}

setInterval(drawMatrix, 35);
</script>

</body>
</html>
