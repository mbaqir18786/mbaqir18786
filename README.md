<svg width="1200" height="320" viewBox="0 0 1200 320" xmlns="http://www.w3.org/2000/svg">
  <defs>
    <pattern id="grid" width="24" height="24" patternUnits="userSpaceOnUse">
      <path d="M 24 0 L 0 0 0 24" fill="none" stroke="#1e293b" stroke-width="1"/>
    </pattern>
    <linearGradient id="bg" x1="0%" y1="0%" x2="100%" y2="100%">
      <stop offset="0%" stop-color="#0b1220"/>
      <stop offset="100%" stop-color="#0f172a"/>
    </linearGradient>
    <linearGradient id="accent" x1="0%" y1="0%" x2="100%" y2="0%">
      <stop offset="0%" stop-color="#ea580c"/>
      <stop offset="100%" stop-color="#fb923c"/>
    </linearGradient>
  </defs>

  <!-- background -->
  <rect width="1200" height="320" fill="url(#bg)"/>
  <rect width="1200" height="320" fill="url(#grid)" opacity="0.5"/>

  <!-- corner crop marks, engineering-drawing style -->
  <g stroke="#ea580c" stroke-width="2" opacity="0.9">
    <line x1="24" y1="24" x2="64" y2="24"><animate attributeName="x2" from="24" to="64" dur="0.6s" fill="freeze"/></line>
    <line x1="24" y1="24" x2="24" y2="64"><animate attributeName="y2" from="24" to="64" dur="0.6s" fill="freeze"/></line>

    <line x1="1176" y1="24" x2="1136" y2="24"><animate attributeName="x2" from="1176" to="1136" dur="0.6s" fill="freeze"/></line>
    <line x1="1176" y1="24" x2="1176" y2="64"><animate attributeName="y2" from="24" to="64" dur="0.6s" fill="freeze"/></line>

    <line x1="24" y1="296" x2="64" y2="296"><animate attributeName="x2" from="24" to="64" dur="0.6s" fill="freeze"/></line>
    <line x1="24" y1="296" x2="24" y2="256"><animate attributeName="y2" from="296" to="256" dur="0.6s" fill="freeze"/></line>

    <line x1="1176" y1="296" x2="1136" y2="296"><animate attributeName="x2" from="1176" to="1136" dur="0.6s" fill="freeze"/></line>
    <line x1="1176" y1="296" x2="1176" y2="256"><animate attributeName="y2" from="296" to="256" dur="0.6s" fill="freeze"/></line>
  </g>

  <!-- animated draw-in horizontal baseline under name -->
  <line x1="80" y1="190" x2="1120" y2="190" stroke="url(#accent)" stroke-width="3" stroke-dasharray="1040" stroke-dashoffset="1040">
    <animate attributeName="stroke-dashoffset" from="1040" to="0" dur="1.4s" begin="0.3s" fill="freeze" calcMode="spline" keySplines="0.4 0 0.2 1"/>
  </line>

  <!-- small dimension ticks along the baseline -->
  <g stroke="#fb923c" stroke-width="1.5" opacity="0">
    <animate xlink:href="#ticks" attributeName="opacity" to="1" begin="1.7s" dur="0.4s" fill="freeze"/>
    <g id="ticks">
      <line x1="80" y1="184" x2="80" y2="196"/>
      <line x1="1120" y1="184" x2="1120" y2="196"/>
    </g>
  </g>

  <!-- name -->
  <text x="80" y="150" font-family="'Courier New', monospace" font-size="46" font-weight="700" fill="#f8fafc" opacity="0">
    <animate attributeName="opacity" from="0" to="1" dur="0.8s" begin="0.2s" fill="freeze"/>
    <animate attributeName="y" from="165" to="150" dur="0.8s" begin="0.2s" fill="freeze" calcMode="spline" keySplines="0.2 0 0.2 1"/>
    Mohammed Baqir Bandarkar
  </text>

  <!-- role line, typewriter reveal via clip -->
  <clipPath id="typeClip">
    <rect x="0" y="0" height="40" width="0">
      <animate attributeName="width" from="0" to="760" dur="2.2s" begin="1.6s" fill="freeze"/>
    </rect>
  </clipPath>
  <text x="80" y="222" font-family="'Courier New', monospace" font-size="20" fill="#ea580c" clip-path="url(#typeClip)">
    &gt; Tech Head @ Alumni Cell — Full Stack + AI/ML — building things people actually use
  </text>
  <rect x="80" y="205" width="2" height="22" fill="#ea580c">
    <animate attributeName="x" from="80" to="840" dur="2.2s" begin="1.6s" fill="freeze"/>
    <animate attributeName="opacity" values="1;0;1" dur="0.8s" begin="1.6s" repeatCount="indefinite"/>
  </rect>

  <!-- subtitle tag, engineering label style -->
  <g opacity="0">
    <animate attributeName="opacity" from="0" to="1" dur="0.6s" begin="3.9s" fill="freeze"/>
    <rect x="80" y="252" width="150" height="26" rx="3" fill="none" stroke="#334155" stroke-width="1"/>
    <text x="90" y="269" font-family="'Courier New', monospace" font-size="12" fill="#94a3b8">REV. 2028 · KJSCE</text>
  </g>

  <!-- floating accent dot, subtle idle motion -->
  <circle cx="1080" cy="70" r="4" fill="#ea580c">
    <animate attributeName="cy" values="70;62;70" dur="3s" repeatCount="indefinite"/>
    <animate attributeName="opacity" values="0.4;1;0.4" dur="3s" repeatCount="indefinite"/>
  </circle>
  <circle cx="1105" cy="90" r="3" fill="#fb923c">
    <animate attributeName="cy" values="90;80;90" dur="2.4s" repeatCount="indefinite"/>
    <animate attributeName="opacity" values="0.3;0.9;0.3" dur="2.4s" repeatCount="indefinite"/>
  </circle>
</svg>
