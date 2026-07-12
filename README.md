<svg xmlns="http://www.w3.org/2000/svg" viewBox="0 0 800 350" width="100%" height="100%">
  <defs>
    <linearGradient id="bg" x1="0%" y1="0%" x2="100%" y2="100%">
      <stop offset="0%" stop-color="#0a0a0a"/>
      <stop offset="50%" stop-color="#111111"/>
      <stop offset="100%" stop-color="#050505"/>
    </linearGradient>
    
    <linearGradient id="glow" x1="0%" y1="0%" x2="100%" y2="0%">
      <stop offset="0%" stop-color="#00FF99"/>
      <stop offset="100%" stop-color="#0066FF"/>
    </linearGradient>

    <pattern id="grid" width="40" height="40" patternUnits="userSpaceOnUse">
      <path d="M 40 0 L 0 0 0 40" fill="none" stroke="#ffffff" stroke-width="0.5" stroke-opacity="0.05"/>
    </pattern>

    <style>
      .grid-bg { animation: pan 20s linear infinite; }
      .title { font-family: -apple-system, BlinkMacSystemFont, "Segoe UI", Roboto, Helvetica, Arial, sans-serif; font-size: 38px; font-weight: 800; fill: url(#glow); }
      .subtitle { font-family: monospace; font-size: 16px; fill: #888; animation: type 4s steps(40, end) infinite alternate; overflow: hidden; white-space: nowrap; }
      .particle { fill: #00FF99; opacity: 0.5; animation: float 6s ease-in-out infinite; }
      
      @keyframes pan { 0% { transform: translateY(0); } 100% { transform: translateY(-40px); } }
      @keyframes float { 0%, 100% { transform: translateY(0) scale(1); opacity: 0.3; } 50% { transform: translateY(-20px) scale(1.5); opacity: 0.8; } }
      @keyframes pulse { 0%, 100% { filter: drop-shadow(0 0 10px rgba(0,255,153,0.5)); } 50% { filter: drop-shadow(0 0 25px rgba(0,255,153,0.9)); } }
    </style>
  </defs>

  <!-- Background -->
  <rect width="100%" height="100%" fill="url(#bg)"/>
  <rect width="100%" height="150%" fill="url(#grid)" class="grid-bg"/>

  <!-- Floating Particles -->
  <circle cx="100" cy="250" r="2" class="particle" style="animation-delay: 0s;"/>
  <circle cx="700" cy="150" r="3" class="particle" style="animation-delay: 2s;"/>
  <circle cx="400" cy="300" r="1.5" class="particle" style="animation-delay: 4s;"/>
  <circle cx="200" cy="100" r="2.5" class="particle" style="animation-delay: 1s;"/>

  <!-- Glassmorphism Card -->
  <rect x="50" y="50" width="700" height="250" rx="15" fill="rgba(255, 255, 255, 0.02)" stroke="rgba(255, 255, 255, 0.05)" stroke-width="1" style="backdrop-filter: blur(10px);"/>

  <!-- Breathing Avatar Circle -->
  <circle cx="400" cy="120" r="45" fill="none" stroke="url(#glow)" stroke-width="3" style="animation: pulse 3s infinite;"/>
  <text x="400" y="130" font-family="monospace" font-size="24" fill="#fff" text-anchor="middle">👨‍💻</text>

  <!-- Text -->
  <text x="400" y="210" text-anchor="middle" class="title">ABISHEK A.</text>
  <text x="400" y="245" text-anchor="middle" class="subtitle">> Architecting the Future of HealthTech_</text>
  
  <!-- UI Accents -->
  <rect x="60" y="60" width="10" height="10" rx="5" fill="#FF5F56"/>
  <rect x="80" y="60" width="10" height="10" rx="5" fill="#FFBD2E"/>
  <rect x="100" y="60" width="10" height="10" rx="5" fill="#27C93F"/>
</svg>
