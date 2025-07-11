<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8" />
  <meta name="viewport" content="width=device-width, initial-scale=1.0"/>
  <title>To Kate</title>

  <!-- Google Fonts -->
  <link href="https://fonts.googleapis.com/css2?family=Playfair+Display:wght@600&family=Quicksand:wght@400;500&display=swap" rel="stylesheet">

  <style>
    body {
      margin: 0;
      padding: 0;
      background: linear-gradient(to bottom right, #f9f3f3, #e3d7f1);
      font-family: 'Quicksand', sans-serif;
      color: #2d2d2d;
      display: flex;
      flex-direction: column;
      align-items: center;
      min-height: 100vh;
    }

    .container {
      max-width: 700px;
      background: #fff9f9;
      padding: 2.5rem;
      margin: 3rem;
      border-radius: 20px;
      box-shadow: 0 10px 40px rgba(114, 75, 144, 0.15);
      text-align: center;
      border: 1px solid #e0c8e6;
    }

    h1 {
      font-family: 'Playfair Display', serif;
      font-size: 2.8rem;
      margin-bottom: 1.5rem;
      color: #8e44ad;
      letter-spacing: 1px;
    }

    p {
      font-size: 1.15rem;
      line-height: 1.9;
      margin-bottom: 1.5rem;
      color: #4e3b58;
    }

    .highlight {
      color: #d63384;
      font-weight: 500;
      font-size: 1.2rem;
    }

    .signature {
      font-style: italic;
      color: #6c5a7c;
      margin-top: 2rem;
      font-size: 1.05rem;
    }

    .footer {
      margin-top: 2rem;
      font-size: 0.95rem;
      color: #998aa8;
      font-style: italic;
    }

    @media (max-width: 768px) {
      .container {
        margin: 1rem;
        padding: 2rem;
      }
    }
    .heart, .petal {
  position: fixed;
  top: -50px;
  animation: fall 10s linear infinite;
  opacity: 0.8;
  pointer-events: none;
  z-index: 0;
}

.heart::before, .heart::after {
  content: "";
  position: absolute;
  width: 20px;
  height: 20px;
  background: #ff6b81;
  border-radius: 50%;
}

.heart::before {
  top: 0;
  left: 10px;
}

.heart::after {
  top: 10px;
  left: 0;
  transform: rotate(-45deg);
}

.petal {
  width: 20px;
  height: 20px;
  background: radial-gradient(circle at center, #e75480 0%, #d6336c 80%);
  border-radius: 50% 50% 50% 0;
  transform: rotate(45deg);
}

@keyframes fall {
  0% {
    transform: translateY(-50px) rotate(0deg);
  }
  100% {
    transform: translateY(100vh) rotate(360deg);
  }
}

  </style>
</head>
<script>
  function createFloatingElement(type) {
    const el = document.createElement('div');
    el.classList.add(type);

    el.style.left = Math.random() * 100 + 'vw';
    el.style.animationDuration = (5 + Math.random() * 5) + 's';
    el.style.opacity = Math.random() * 0.7 + 0.3;
    el.style.transform = `scale(${Math.random() + 0.5})`;

    document.body.appendChild(el);

    setTimeout(() => {
      el.remove();
    }, 10000);
  }

  setInterval(() => {
    createFloatingElement('hearts');
    createFloatingElement('petal');
  }, 600);
</script>
<body>
  <div class="container">
    <h1>Heyyy Kate,</h1>

    <p>
      I’ve thought a lot about whether or not to try and say something.
    </p>

    <p>
      When we met, being around you felt different, it was calm, exciting and enchanting. I genuinely felt a spark that I hoped wasn't just in my head. 
    </p>

    <p>
      Lately though, I’ve been met with silence and I don’t know if I did something wrong. If I did, I’m sorry. That was never my intention. You deserve someone who respects your pace (in case I was going too fast), and who would never want to make you uncomfortable.
    </p>

    <p>
      This isn't me chasing or demanding anything. It's just my way of honoring what I felt for you.
    </p>

    <p>
      I definitely won't regret opening up to you, but I was really optimistic. In case you stopped feeling the same way, please lemme know yeah.
    </p>

    <p class="highlight">
      But if by any chance you're still out there thinking about us, my heart is still open to you.
    </p>

    <div class="signature">
      – Miles 
    </div>

    <div class="footer">
      “Sometimes the right words are the ones that free you, even if they don’t bring them back.”
    </div>
  </div>
</body>
</html>
