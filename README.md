<svg width="1200" height="300" viewBox="0 0 1200 300" xmlns="http://www.w3.org/2000/svg">
  <defs>
    <linearGradient id="bgGrad" x1="0%" y1="0%" x2="100%" y2="100%">
      <stop offset="0%" stop-color="#0f0c29"/>
      <stop offset="45%" stop-color="#302b63"/>
      <stop offset="100%" stop-color="#24243e"/>
    </linearGradient>
    <radialGradient id="glow" cx="50%" cy="50%" r="50%">
      <stop offset="0%" stop-color="#A855F7" stop-opacity="0.55"/>
      <stop offset="100%" stop-color="#A855F7" stop-opacity="0"/>
    </radialGradient>
    <linearGradient id="ringGrad" x1="0%" y1="0%" x2="100%" y2="0%">
      <stop offset="0%" stop-color="#A855F7"/>
      <stop offset="50%" stop-color="#EC4899"/>
      <stop offset="100%" stop-color="#38BDF8"/>
    </linearGradient>
    <linearGradient id="textGrad" x1="0%" y1="0%" x2="100%" y2="0%">
      <stop offset="0%" stop-color="#F5D0FE"/>
      <stop offset="50%" stop-color="#E9D5FF"/>
      <stop offset="100%" stop-color="#BAE6FD"/>
    </linearGradient>
    <filter id="softBlur" x="-50%" y="-50%" width="200%" height="200%">
      <feGaussianBlur stdDeviation="3"/>
    </filter>
  </defs>

  <!-- background -->
  <rect width="1200" height="300" fill="url(#bgGrad)"/>

  <!-- soft ambient glow, pulsing -->
  <circle cx="1000" cy="150" r="220" fill="url(#glow)">
    <animate attributeName="r" values="200;240;200" dur="4s" repeatCount="indefinite"/>
    <animate attributeName="opacity" values="0.6;0.9;0.6" dur="4s" repeatCount="indefinite"/>
  </circle>
  <circle cx="150" cy="230" r="140" fill="url(#glow)" opacity="0.5">
    <animate attributeName="r" values="120;150;120" dur="5s" repeatCount="indefinite"/>
  </circle>

  <!-- scattered twinkling stars -->
  <g fill="#F5D0FE">
    <circle cx="80" cy="50" r="2"><animate attributeName="opacity" values="0.2;1;0.2" dur="2.1s" repeatCount="indefinite"/></circle>
    <circle cx="220" cy="30" r="1.6"><animate attributeName="opacity" values="1;0.2;1" dur="2.6s" repeatCount="indefinite"/></circle>
    <circle cx="340" cy="70" r="2.2"><animate attributeName="opacity" values="0.3;1;0.3" dur="3.1s" repeatCount="indefinite"/></circle>
    <circle cx="60" cy="180" r="1.8"><animate attributeName="opacity" values="1;0.3;1" dur="2.4s" repeatCount="indefinite"/></circle>
    <circle cx="900" cy="40" r="2"><animate attributeName="opacity" values="0.2;1;0.2" dur="2.9s" repeatCount="indefinite"/></circle>
    <circle cx="1050" cy="70" r="1.6"><animate attributeName="opacity" values="1;0.2;1" dur="2.2s" repeatCount="indefinite"/></circle>
    <circle cx="1140" cy="200" r="2.2"><animate attributeName="opacity" values="0.3;1;0.3" dur="3.4s" repeatCount="indefinite"/></circle>
    <circle cx="980" cy="250" r="1.8"><animate attributeName="opacity" values="1;0.3;1" dur="2.7s" repeatCount="indefinite"/></circle>
  </g>

  <!-- rotating tech-ring emblem, right side -->
  <g transform="translate(1000,150)">
    <g>
      <animateTransform attributeName="transform" type="rotate" from="0 0 0" to="360 0 0" dur="18s" repeatCount="indefinite"/>
      <circle r="95" fill="none" stroke="url(#ringGrad)" stroke-width="2.5" stroke-dasharray="10 8" opacity="0.85"/>
    </g>
    <g>
      <animateTransform attributeName="transform" type="rotate" from="360 0 0" to="0 0 0" dur="12s" repeatCount="indefinite"/>
      <circle r="72" fill="none" stroke="#38BDF8" stroke-width="1.5" stroke-dasharray="3 6" opacity="0.7"/>
    </g>
    <g>
      <animateTransform attributeName="transform" type="rotate" from="0 0 0" to="360 0 0" dur="26s" repeatCount="indefinite"/>
      <circle r="115" fill="none" stroke="#EC4899" stroke-width="1" stroke-dasharray="1 12" opacity="0.6"/>
    </g>

    <!-- orbiting sparkle nodes -->
    <g>
      <animateTransform attributeName="transform" type="rotate" from="0 0 0" to="360 0 0" dur="8s" repeatCount="indefinite"/>
      <circle cx="95" cy="0" r="4" fill="#F5D0FE"/>
    </g>
    <g>
      <animateTransform attributeName="transform" type="rotate" from="180 0 0" to="540 0 0" dur="8s" repeatCount="indefinite"/>
      <circle cx="95" cy="0" r="4" fill="#38BDF8"/>
    </g>
    <g>
      <animateTransform attributeName="transform" type="rotate" from="90 0 0" to="450 0 0" dur="14s" repeatCount="indefinite"/>
      <circle cx="72" cy="0" r="3" fill="#EC4899"/>
    </g>
    <g>
      <animateTransform attributeName="transform" type="rotate" from="270 0 0" to="-90 0 0" dur="14s" repeatCount="indefinite"/>
      <circle cx="72" cy="0" r="3" fill="#A855F7"/>
    </g>

    <!-- core AI glyph: neural node cluster -->
    <g stroke="url(#ringGrad)" stroke-width="1.5" fill="none" opacity="0.9">
      <line x1="0" y1="0" x2="-30" y2="-18"/>
      <line x1="0" y1="0" x2="30" y2="-18"/>
      <line x1="0" y1="0" x2="-30" y2="18"/>
      <line x1="0" y1="0" x2="30" y2="18"/>
      <line x1="0" y1="0" x2="0" y2="-34"/>
    </g>
    <circle r="10" fill="#0f0c29" stroke="url(#ringGrad)" stroke-width="2"/>
    <circle cx="-30" cy="-18" r="4" fill="#38BDF8"/>
    <circle cx="30" cy="-18" r="4" fill="#EC4899"/>
    <circle cx="-30" cy="18" r="4" fill="#A855F7"/>
    <circle cx="30" cy="18" r="4" fill="#F5D0FE"/>
    <circle cx="0" cy="-34" r="4" fill="#38BDF8"/>
    <circle r="4" fill="#F5D0FE">
      <animate attributeName="opacity" values="0.5;1;0.5" dur="1.8s" repeatCount="indefinite"/>
    </circle>
  </g>

  <!-- falling sakura petals -->
  <g fill="#F472B6" opacity="0.85">
    <ellipse cx="0" cy="0" rx="6" ry="3.5">
      <animateTransform attributeName="transform" type="translate" values="120,-20; 90,320" dur="7s" repeatCount="indefinite"/>
      <animateTransform attributeName="transform" type="rotate" values="0;360" dur="3s" repeatCount="indefinite" additive="sum"/>
    </ellipse>
    <ellipse cx="0" cy="0" rx="5" ry="3">
      <animateTransform attributeName="transform" type="translate" values="260,-30; 300,330" dur="9s" repeatCount="indefinite"/>
      <animateTransform attributeName="transform" type="rotate" values="0;-360" dur="4s" repeatCount="indefinite" additive="sum"/>
    </ellipse>
    <ellipse cx="0" cy="0" rx="6" ry="3.5">
      <animateTransform attributeName="transform" type="translate" values="450,-25; 420,320" dur="8s" repeatCount="indefinite"/>
      <animateTransform attributeName="transform" type="rotate" values="0;360" dur="3.5s" repeatCount="indefinite" additive="sum"/>
    </ellipse>
    <ellipse cx="0" cy="0" rx="5" ry="3">
      <animateTransform attributeName="transform" type="translate" values="30,-15; 60,310" dur="6.5s" repeatCount="indefinite"/>
      <animateTransform attributeName="transform" type="rotate" values="0;-360" dur="3s" repeatCount="indefinite" additive="sum"/>
    </ellipse>
  </g>

  <!-- name + role text -->
  <text x="60" y="140" font-family="'Trebuchet MS', Verdana, sans-serif" font-size="46" font-weight="700" fill="url(#textGrad)">
    Revati G Chavadal
  </text>
  <text x="60" y="180" font-family="'Trebuchet MS', Verdana, sans-serif" font-size="21" fill="#C4B5FD" letter-spacing="1.5">
    AI / ML DEVELOPER &#183; PYTHON &#183; FASTAPI
  </text>

  <!-- animated underline accent -->
  <rect x="60" y="196" width="0" height="4" rx="2" fill="url(#ringGrad)">
    <animate attributeName="width" values="0;340;340" keyTimes="0;0.6;1" dur="2.5s" repeatCount="indefinite"/>
  </rect>

  <!-- tagline -->
  <text x="60" y="235" font-family="'Trebuchet MS', Verdana, sans-serif" font-size="15" fill="#93C5FD" opacity="0.9">
    building real-world AI solutions, one commit at a time
  </text>
</svg>
