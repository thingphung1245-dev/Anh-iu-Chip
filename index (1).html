<!DOCTYPE html>
<html lang="vi">
<head>
  <meta charset="UTF-8" />
  <meta name="viewport" content="width=device-width, initial-scale=1.0" />
  <title>I Love You ❤️</title>
  <style>
    * { margin: 0; padding: 0; box-sizing: border-box; }
    body {
      background: #000;
      display: flex;
      flex-direction: column;
      align-items: center;
      justify-content: center;
      min-height: 100vh;
      overflow: hidden;
      font-family: sans-serif;
    }
    canvas { display: block; }
    #message {
      color: #ff69b4;
      font-size: 18px;
      letter-spacing: 3px;
      margin-top: 16px;
      opacity: 0;
      animation: fadeIn 2s ease 1s forwards;
      text-shadow: 0 0 12px rgba(255,105,180,0.8);
    }
    @keyframes fadeIn { to { opacity: 1; } }
  </style>
</head>
<body>
  <canvas id="c"></canvas>
  <div id="message">✦ Made with love ✦</div>

  <script>
    const canvas = document.getElementById('c');
    const ctx = canvas.getContext('2d');

    function resize() {
      const size = Math.min(window.innerWidth, window.innerHeight, 700);
      canvas.width = size;
      canvas.height = size * 0.75;
    }
    resize();
    window.addEventListener('resize', resize);

    function heartX(t) { return 16 * Math.pow(Math.sin(t), 3); }
    function heartY(t) {
      return -(13*Math.cos(t) - 5*Math.cos(2*t) - 2*Math.cos(3*t) - Math.cos(4*t));
    }

    const TEXTS = ['I Love You', 'I Love You', 'I ❤ You', 'Love You', 'I Love You'];
    const N = 300;
    const particles = [];

    for (let i = 0; i < N; i++) {
      const t = (i / N) * Math.PI * 2;
      particles.push({
        t,
        offset: Math.random() * Math.PI * 2,
        speed: 0.03 + Math.random() * 0.02,
        size: 8 + Math.random() * 6,
        label: TEXTS[Math.floor(Math.random() * TEXTS.length)],
        rotDir: Math.random() > 0.5 ? 1 : -1,
      });
    }

    let frame = 0;

    function draw() {
      const W = canvas.width, H = canvas.height;
      ctx.clearRect(0, 0, W, H);
      ctx.fillStyle = '#000';
      ctx.fillRect(0, 0, W, H);

      const pulse = 1 + 0.05 * Math.sin(frame * 0.04);
      const scale = (W / 60) * pulse;
      const cx = W / 2;
      const cy = H / 2;

      particles.forEach((p) => {
        const x = cx + heartX(p.t) * scale;
        const y = cy + heartY(p.t) * scale;

        const alpha = 0.55 + 0.45 * Math.sin(frame * p.speed + p.offset);
        const rot = p.rotDir * frame * 0.008 + p.t * 0.2;

        ctx.save();
        ctx.translate(x, y);
        ctx.rotate(rot);
        ctx.font = `${p.size}px sans-serif`;
        ctx.fillStyle = `rgba(255, 105, 180, ${alpha})`;
        ctx.shadowColor = 'rgba(255, 80, 150, 0.9)';
        ctx.shadowBlur = 10;
        ctx.fillText(p.label, 0, 0);
        ctx.restore();
      });

      frame++;
      requestAnimationFrame(draw);
    }

    draw();
  </script>
</body>
</html>
