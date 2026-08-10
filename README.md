<svg width="1200" height="340" viewBox="0 0 1200 340" xmlns="http://www.w3.org/2000/svg" xmlns:xlink="http://www.w3.org/1999/xlink">
  <defs>
    <pattern id="grid" width="26" height="26" patternUnits="userSpaceOnUse">
      <path d="M 26 0 L 0 0 0 26" fill="none" stroke="#17233a" stroke-width="1"/>
    </pattern>
    <linearGradient id="bg" x1="0%" y1="0%" x2="100%" y2="100%">
      <stop offset="0%" stop-color="#0a0f1c"/>
      <stop offset="55%" stop-color="#0d1626"/>
      <stop offset="100%" stop-color="#0a1420"/>
    </linearGradient>
    <linearGradient id="accent" x1="0%" y1="0%" x2="100%" y2="0%">
      <stop offset="0%" stop-color="#ea580c"/>
      <stop offset="55%" stop-color="#fb923c"/>
      <stop offset="100%" stop-color="#22d3ee"/>
    </linearGradient>
    <radialGradient id="glow" cx="50%" cy="50%" r="50%">
      <stop offset="0%" stop-color="#ea580c" stop-opacity="0.35"/>
      <stop offset="100%" stop-color="#ea580c" stop-opacity="0"/>
    </radialGradient>
    <radialGradient id="glowCyan" cx="50%" cy="50%" r="50%">
      <stop offset="0%" stop-color="#22d3ee" stop-opacity="0.28"/>
      <stop offset="100%" stop-color="#22d3ee" stop-opacity="0"/>
    </radialGradient>
    <clipPath id="nameClip">
      <rect x="0" y="0" width="0" height="70">
        <animate attributeName="width" from="0" to="760" dur="1s" begin="0.15s" fill="freeze" calcMode="spline" keySplines="0.3 0 0.15 1"/>
      </rect>
    </clipPath>
  </defs>

  <rect width="1200" height="340" fill="url(#bg)"/>
  <rect width="1200" height="340" fill="url(#grid)" opacity="0.55"/>
  <circle cx="1020" cy="80" r="220" fill="url(#glow)"/>
  <circle cx="120" cy="290" r="180" fill="url(#glowCyan)"/>

  <!-- corner crop marks -->
  <g stroke="#ea580c" stroke-width="2" opacity="0.9">
    <line x1="24" y1="24" x2="24" y2="24"><animate attributeName="x2" from="24" to="64" dur="0.5s" fill="freeze"/></line>
    <line x1="24" y1="24" x2="24" y2="24"><animate attributeName="y2" from="24" to="64" dur="0.5s" fill="freeze"/></line>
    <line x1="1176" y1="24" x2="1176" y2="24"><animate attributeName="x2" from="1176" to="1136" dur="0.5s" fill="freeze"/></line>
    <line x1="1176" y1="24" x2="1176" y2="24"><animate attributeName="y2" from="24" to="64" dur="0.5s" fill="freeze"/></line>
    <line x1="24" y1="316" x2="24" y2="316"><animate attributeName="x2" from="24" to="64" dur="0.5s" fill="freeze"/></line>
    <line x1="24" y1="316" x2="24" y2="316"><animate attributeName="y2" from="316" to="276" dur="0.5s" fill="freeze"/></line>
    <line x1="1176" y1="316" x2="1176" y2="316"><animate attributeName="x2" from="1176" to="1136" dur="0.5s" fill="freeze"/></line>
    <line x1="1176" y1="316" x2="1176" y2="316"><animate attributeName="y2" from="316" to="276" dur="0.5s" fill="freeze"/></line>
  </g>

  <!-- rotating compass / drafting icon -->
  <g transform="translate(1100,70)">
    <g>
      <animateTransform attributeName="transform" type="rotate" from="0 0 0" to="360 0 0" dur="14s" repeatCount="indefinite"/>
      <circle r="34" fill="none" stroke="#22d3ee" stroke-width="1.4" stroke-dasharray="4 5" opacity="0.8"/>
      <line x1="0" y1="-34" x2="0" y2="-24" stroke="#fb923c" stroke-width="2"/>
      <line x1="0" y1="24" x2="0" y2="34" stroke="#fb923c" stroke-width="2"/>
      <line x1="-34" y1="0" x2="-24" y2="0" stroke="#fb923c" stroke-width="2"/>
      <line x1="24" y1="0" x2="34" y2="0" stroke="#fb923c" stroke-width="2"/>
    </g>
    <circle r="5" fill="#ea580c"/>
  </g>

  <!-- name -->
  <g clip-path="url(#nameClip)">
    <text x="80" y="165" font-family="'Courier New', monospace" font-size="48" font-weight="700" fill="#f8fafc">Mohammed Baqir Bandarkar</text>
  </g>

  <!-- baseline draw-in -->
  <line x1="80" y1="192" x2="80" y2="192" stroke="url(#accent)" stroke-width="3">
    <animate attributeName="x2" from="80" to="900" dur="1s" begin="1.1s" fill="freeze" calcMode="spline" keySplines="0.3 0 0.15 1"/>
  </line>
  <g stroke="#fb923c" stroke-width="1.5" opacity="0">
    <animate attributeName="opacity" to="1" begin="2.1s" dur="0.3s" fill="freeze"/>
    <line x1="80" y1="186" x2="80" y2="198"/>
    <line x1="900" y1="186" x2="900" y2="198"/>
  </g>

  <!-- role rotator -->
  <g font-family="'Courier New', monospace" font-size="21" fill="#fb923c">
    <text x="80" y="228" opacity="0">&gt; Tech Head @ Alumni Cell
      <animate attributeName="opacity" values="0;1;1;0;0;0;0;0" keyTimes="0;0.05;0.22;0.27;1;1;1;1" dur="9s" begin="2.4s" repeatCount="indefinite"/>
    </text>
    <text x="80" y="228" opacity="0">&gt; Full-Stack + AI/ML Engineer
      <animate attributeName="opacity" values="0;0;0;1;1;0;0;0" keyTimes="0;0.25;0.30;0.33;0.52;0.55;1;1" dur="9s" begin="2.4s" repeatCount="indefinite"/>
    </text>
    <text x="80" y="228" opacity="0" fill="#22d3ee">&gt; Building KickStart 2026
      <animate attributeName="opacity" values="0;0;0;0;0;1;1;0;0" keyTimes="0;0.50;0.55;0.58;0.60;0.63;0.80;0.83;1" dur="9s" begin="2.4s" repeatCount="indefinite"/>
    </text>
    <text x="80" y="228" opacity="0">&gt; Product-minded, not portfolio-minded
      <animate attributeName="opacity" values="0;0;0;0;0;0;0;1;1;0" keyTimes="0;0.80;0.85;0.86;0.87;0.88;0.89;0.92;0.98;1" dur="9s" begin="2.4s" repeatCount="indefinite"/>
    </text>
    <rect x="0" y="211" width="2" height="20" fill="#fb923c">
      <animate attributeName="x" values="410;410" dur="0.1s"/>
      <animate attributeName="opacity" values="1;0;1" dur="0.9s" repeatCount="indefinite"/>
      <animate attributeName="x" from="80" to="80" dur="0.1s" begin="0s" fill="freeze"/>
    </rect>
  </g>

  <!-- status pill -->
  <g opacity="0">
    <animate attributeName="opacity" to="1" begin="2.6s" dur="0.5s" fill="freeze"/>
    <rect x="80" y="258" width="242" height="30" rx="15" fill="none" stroke="#22d3ee" stroke-width="1.2"/>
    <circle cx="98" cy="273" r="4" fill="#4ade80">
      <animate attributeName="opacity" values="1;0.25;1" dur="1.6s" repeatCount="indefinite"/>
    </circle>
    <text x="112" y="278" font-family="'Courier New', monospace" font-size="13" fill="#cbd5e1" letter-spacing="0.5">OPEN TO WEB-DEV INTERNSHIPS</text>
  </g>

  <!-- rev stamp -->
  <g opacity="0">
    <animate attributeName="opacity" to="1" begin="3.2s" dur="0.5s" fill="freeze"/>
    <rect x="1000" y="258" width="120" height="28" rx="3" fill="none" stroke="#334155" stroke-width="1"/>
    <text x="1010" y="277" font-family="'Courier New', monospace" font-size="12" fill="#94a3b8">REV.2028 · KJSCE</text>
  </g>

  <!-- floating dots -->
  <circle cx="960" cy="140" r="3.5" fill="#ea580c">
    <animate attributeName="cy" values="140;128;140" dur="3s" repeatCount="indefinite"/>
    <animate attributeName="opacity" values="0.4;1;0.4" dur="3s" repeatCount="indefinite"/>
  </circle>
  <circle cx="990" cy="165" r="2.5" fill="#22d3ee">
    <animate attributeName="cy" values="165;153;165" dur="2.3s" repeatCount="indefinite"/>
    <animate attributeName="opacity" values="0.3;0.9;0.3" dur="2.3s" repeatCount="indefinite"/>
  </circle>
  <circle cx="140" cy="90" r="2.5" fill="#fb923c">
    <animate attributeName="cy" values="90;78;90" dur="2.8s" repeatCount="indefinite"/>
    <animate attributeName="opacity" values="0.3;0.9;0.3" dur="2.8s" repeatCount="indefinite"/>
  </circle>
</svg>
