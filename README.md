<div align="center">

<!-- Texto Animado -->
<img src="cooltext478830476046430.gif" alt="Meu Texto Animado">

---
<!DOCTYPE html>
<html lang="en">
<head>
<meta charset="UTF-8">
<title>Animação Estrelas Neon</title>
<style>
  body {
    margin: 0;
    overflow: hidden;
    background: black;
  }
  canvas {
    display: block;
  }
</style>
</head>
<body>
<canvas id="starCanvas"></canvas>
<script>
  const canvas = document.getElementById('starCanvas');
  const ctx = canvas.getContext('2d');
  canvas.width = window.innerWidth;
  canvas.height = window.innerHeight;

  const stars = [];
  const numStars = 100;

  for (let i = 0; i < numStars; i++) {
    stars.push({
      x: Math.random() * canvas.width,
      y: Math.random() * canvas.height,
      radius: Math.random() * 2,
      speedX: Math.random() * 2 - 1,
      speedY: Math.random() * 2 - 1
    });
  }

  function drawStars() {
    ctx.clearRect(0, 0, canvas.width, canvas.height);
    ctx.fillStyle = "white";
    stars.forEach(star => {
      ctx.beginPath();
      ctx.arc(star.x, star.y, star.radius, 0, Math.PI * 2);
      ctx.fill();
      star.x += star.speedX;
      star.y += star.speedY;

      if (star.x < 0 || star.x > canvas.width) star.speedX *= -1;
      if (star.y < 0 || star.y > canvas.height) star.speedY *= -1;
    });
  }

  function animate() {
    drawStars();
    requestAnimationFrame(animate);
  }

  animate();
</script>
</body>
</html>
---
<!-- Gráfico de Linguagens -->
[![Top Langs](https://github-readme-stats.vercel.app/api/top-langs/?username=Eduardovass04&layout=compact&langs_count=10&theme=radical)](https://github.com/anuraghazra/github-readme-stats)

---

<!-- Botão Instagram -->
[![Instagram](https://img.shields.io/badge/-Instagram-%23E4405F.svg?style=for-the-badge&logo=Instagram&logoColor=white)](https://www.instagram.com/eduardovasconcelos04)

</div>
