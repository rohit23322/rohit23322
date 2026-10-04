<div align="center">

<!-- 3D ANIMATED HEADER -->
<svg width="100%" height="420" viewBox="0 0 1200 420"
     xmlns="http://www.w3.org/2000/svg">

  <defs>

    <!-- Background -->
    <linearGradient id="bg" x1="0" y1="0" x2="1" y2="1">
      <stop offset="0%" stop-color="#050816"/>
      <stop offset="50%" stop-color="#0b1026"/>
      <stop offset="100%" stop-color="#02030a"/>
    </linearGradient>

    <!-- Neon gradient -->
    <linearGradient id="neon" x1="0" y1="0" x2="1" y2="1">
      <stop offset="0%" stop-color="#00f5ff"/>
      <stop offset="50%" stop-color="#7c3aed"/>
      <stop offset="100%" stop-color="#ff00c8"/>
    </linearGradient>

    <!-- Glow -->
    <filter id="glow">
      <feGaussianBlur stdDeviation="5" result="blur"/>
      <feMerge>
        <feMergeNode in="blur"/>
        <feMergeNode in="SourceGraphic"/>
      </feMerge>
    </filter>

    <!-- Strong glow -->
    <filter id="strongGlow">
      <feGaussianBlur stdDeviation="10" result="blur"/>
      <feMerge>
        <feMergeNode in="blur"/>
        <feMergeNode in="SourceGraphic"/>
      </feMerge>
    </filter>

    <!-- Grid -->
    <pattern id="grid" width="50" height="50" patternUnits="userSpaceOnUse">
      <path d="M 50 0 L 0 0 0 50"
            fill="none"
            stroke="#00f5ff"
            stroke-opacity="0.12"/>
    </pattern>

  </defs>

  <!-- Background -->
  <rect width="1200" height="420" rx="25" fill="url(#bg)"/>

  <!-- Grid -->
  <rect width="1200" height="420" fill="url(#grid)"/>

  <!-- Animated floating particles -->
  <g fill="#00f5ff" filter="url(#glow)">

    <circle cx="100" cy="80" r="3">
      <animate attributeName="cy"
               values="80;50;80"
               dur="3s"
               repeatCount="indefinite"/>
    </circle>

    <circle cx="1080" cy="120" r="3">
      <animate attributeName="cy"
               values="120;80;120"
               dur="4s"
               repeatCount="indefinite"/>
    </circle>

    <circle cx="950" cy="330" r="2">
      <animate attributeName="cy"
               values="330;290;330"
               dur="3s"
               repeatCount="indefinite"/>
    </circle>

    <circle cx="180" cy="320" r="2">
      <animate attributeName="cy"
               values="320;280;320"
               dur="4s"
               repeatCount="indefinite"/>
    </circle>

  </g>

  <!-- Floating 3D rings -->
  <g fill="none" stroke="url(#neon)" filter="url(#glow)">

    <ellipse cx="180" cy="130"
             rx="75" ry="25"
             stroke-width="2">

      <animateTransform
        attributeName="transform"
        type="rotate"
        from="0 180 130"
        to="360 180 130"
        dur="8s"
        repeatCount="indefinite"/>

    </ellipse>

    <ellipse cx="1020" cy="280"
             rx="80" ry="25"
             stroke-width="2">

      <animateTransform
        attributeName="transform"
        type="rotate"
        from="360 1020 280"
        to="0 1020 280"
        dur="10s"
        repeatCount="indefinite"/>

    </ellipse>

  </g>

  <!-- Main title -->

  <text x="600"
        y="105"
        text-anchor="middle"
        fill="white"
        font-family="Arial, sans-serif"
        font-size="52"
        font-weight="bold"
        filter="url(#glow)">

    ROHIT KHOMANE

    <animate
      attributeName="opacity"
      values="0.7;1;0.7"
      dur="3s"
      repeatCount="indefinite"/>

  </text>

  <!-- Subtitle -->

  <text x="600"
        y="145"
        text-anchor="middle"
        fill="#00f5ff"
        font-family="Arial, sans-serif"
        font-size="22">

    PYTHON DEVELOPER • AI/ML ENGINEER • BACKEND DEVELOPER

  </text>


  <!-- 3D Laptop -->

  <g transform="translate(430,185)">

    <!-- Screen outer -->

    <rect x="0"
          y="0"
          width="340"
          height="170"
          rx="12"
          fill="#111827"
          stroke="url(#neon)"
          stroke-width="4"
          filter="url(#strongGlow)"/>

    <!-- Screen -->

    <rect x="15"
          y="15"
          width="310"
          height="140"
          rx="5"
          fill="#020617"/>

    <!-- Code -->

    <g font-family="monospace"
       font-size="15">

      <text x="35" y="45" fill="#00f5ff">
        &lt;python&gt;
      </text>

      <text x="35" y="70" fill="#a78bfa">
        def
      </text>

      <text x="75" y="70" fill="#ffffff">
        build_ai():
      </text>

      <text x="50" y="95" fill="#22c55e">
        backend = FastAPI()
      </text>

      <text x="50" y="120" fill="#f472b6">
        model = AI()
      </text>

      <text x="50" y="145" fill="#00f5ff">
        return backend + model
      </text>

    </g>

    <!-- Blinking cursor -->

    <rect x="280"
          y="132"
          width="8"
          height="16"
          fill="#00f5ff">

      <animate
        attributeName="opacity"
        values="1;0;1"
        dur="0.8s"
        repeatCount="indefinite"/>

    </rect>

    <!-- Laptop base -->

    <path d="M -35 170 L 375 170 L 420 195 L -80 195 Z"
          fill="#111827"
          stroke="url(#neon)"
          stroke-width="3"/>

    <ellipse cx="170"
             cy="190"
             rx="60"
             ry="5"
             fill="#00f5ff"
             opacity="0.5"/>

  </g>


  <!-- Floating Python symbol -->

  <g transform="translate(270,210)"
     filter="url(#glow)">

    <circle r="38"
            fill="#111827"
            stroke="#00f5ff"
            stroke-width="3">

      <animateTransform
        attributeName="transform"
        type="translate"
        values="0 0;0 -15;0 0"
        dur="3s"
        repeatCount="indefinite"/>

    </circle>

    <text x="0"
          y="10"
          text-anchor="middle"
          fill="#00f5ff"
          font-size="32"
          font-family="Arial"
          font-weight="bold">
      Py
    </text>

  </g>


  <!-- AI symbol -->

  <g transform="translate(880,210)"
     filter="url(#glow)">

    <circle r="38"
            fill="#111827"
            stroke="#ff00c8"
            stroke-width="3">

      <animateTransform
        attributeName="transform"
        type="translate"
        values="0 0;0 15;0 0"
        dur="3.5s"
        repeatCount="indefinite"/>

    </circle>

    <text x="0"
          y="9"
          text-anchor="middle"
          fill="#ff00c8"
          font-size="25"
          font-family="Arial"
          font-weight="bold">
      AI
    </text>

  </g>


  <!-- Bottom tech badges -->

  <g font-family="Arial"
     font-size="16"
     text-anchor="middle">

    <rect x="300" y="380"
          width="130" height="30"
          rx="15"
          fill="#111827"
          stroke="#00f5ff"/>

    <text x="365" y="401"
          fill="#00f5ff">
      Python
    </text>


    <rect x="450" y="380"
          width="130" height="30"
          rx="15"
          fill="#111827"
          stroke="#7c3aed"/>

    <text x="515" y="401"
          fill="#a78bfa">
      FastAPI
    </text>


    <rect x="600" y="380"
          width="130" height="30"
          rx="15"
          fill="#111827"
          stroke="#ff00c8"/>

    <text x="665" y="401"
          fill="#ff00c8">
      AI / ML
    </text>


    <rect x="750" y="380"
          width="130" height="30"
          rx="15"
          fill="#111827"
          stroke="#22c55e"/>

    <text x="815" y="401"
          fill="#22c55e">
      MySQL
    </text>

  </g>

</svg>

</div>
