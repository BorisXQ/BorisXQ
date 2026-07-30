<div align="center">

<!-- HERO BANNER (Animated SVG) -->
<svg xmlns="http://www.w3.org/2000/svg" viewBox="0 0 1200 480" width="100%" height="auto" style="max-width: 100%; height: auto; font-family: -apple-system, BlinkMacSystemFont, 'Segoe UI', Roboto, Helvetica, Arial, sans-serif;">
  <defs>
    <!-- Dark Radial Gradient Background -->
    <radialGradient id="hero-bg" cx="50%" cy="30%" r="85%">
      <stop offset="0%" stop-color="#0F172A" />
      <stop offset="50%" stop-color="#080D1A" />
      <stop offset="100%" stop-color="#020408" />
    </radialGradient>

    <!-- Moving Glow Gradients -->
    <linearGradient id="glow-cyan" x1="0%" y1="0%" x2="100%" y2="100%">
      <stop offset="0%" stop-color="#00F2FE" stop-opacity="0.8">
        <animate attributeName="stop-color" values="#00F2FE;#4FACFE;#00F2FE" dur="6s" repeatCount="indefinite" />
      </stop>
      <stop offset="100%" stop-color="#4FACFE" stop-opacity="0.2" />
    </linearGradient>

    <linearGradient id="glow-blue" x1="100%" y1="0%" x2="0%" y2="100%">
      <stop offset="0%" stop-color="#3B82F6" stop-opacity="0.6">
        <animate attributeName="stop-color" values="#3B82F6;#6366F1;#3B82F6" dur="8s" repeatCount="indefinite" />
      </stop>
      <stop offset="100%" stop-color="#1E3A8A" stop-opacity="0.1" />
    </linearGradient>

    <!-- Grid Pattern -->
    <pattern id="grid" width="40" height="40" patternUnits="userSpaceOnUse">
      <path d="M 40 0 L 0 0 0 40" fill="none" stroke="#1E293B" stroke-width="0.75" stroke-opacity="0.4" />
    </pattern>

    <!-- Conlink Logo Gradient -->
    <linearGradient id="conlink-grad" x1="0%" y1="0%" x2="100%" y2="100%">
      <stop offset="0%" stop-color="#38BDF8" />
      <stop offset="50%" stop-color="#818CF8" />
      <stop offset="100%" stop-color="#C084FC" />
    </linearGradient>

    <!-- Text Metallic Gradient -->
    <linearGradient id="text-grad" x1="0%" y1="0%" x2="0%" y2="100%">
      <stop offset="0%" stop-color="#FFFFFF" />
      <stop offset="100%" stop-color="#94A3B8" />
    </linearGradient>

    <!-- Glass Card Gradient -->
    <linearGradient id="glass-border" x1="0%" y1="0%" x2="100%" y2="100%">
      <stop offset="0%" stop-color="#38BDF8" stop-opacity="0.5" />
      <stop offset="50%" stop-color="#1E293B" stop-opacity="0.2" />
      <stop offset="100%" stop-color="#818CF8" stop-opacity="0.5" />
    </linearGradient>
  </defs>

  <style>
    .hero-title { font-size: 64px; font-weight: 800; fill: url(#text-grad); letter-spacing: -2px; }
    .hero-subtitle { font-size: 20px; font-weight: 500; fill: #38BDF8; letter-spacing: 4px; text-transform: uppercase; }
    .hero-tag { font-size: 14px; font-weight: 400; fill: #94A3B8; letter-spacing: 1px; }
    .pulsing-orb-1 { animation: pulse1 8s ease-in-out infinite alternate; }
    .pulsing-orb-2 { animation: pulse2 10s ease-in-out infinite alternate; }
    .laser-line { stroke-dasharray: 200 1000; animation: dash 4s linear infinite; }
    
    @keyframes pulse1 {
      0% { transform: translate(0px, 0px) scale(1); opacity: 0.3; }
      100% { transform: translate(50px, -30px) scale(1.2); opacity: 0.6; }
    }
    @keyframes pulse2 {
      0% { transform: translate(0px, 0px) scale(1); opacity: 0.2; }
      100% { transform: translate(-40px, 40px) scale(1.3); opacity: 0.5; }
    }
    @keyframes dash {
      0% { stroke-dashoffset: 1200; }
      100% { stroke-dashoffset: 0; }
    }
  </style>

  <!-- Background -->
  <rect width="1200" height="480" fill="url(#hero-bg)" rx="16" />
  <rect width="1200" height="480" fill="url(#grid)" rx="16" />

  <!-- Ambient Glowing Orbs -->
  <circle class="pulsing-orb-1" cx="300" cy="150" r="180" fill="url(#glow-cyan)" filter="blur(60px)" />
  <circle class="pulsing-orb-2" cx="900" cy="320" r="220" fill="url(#glow-blue)" filter="blur(80px)" />

  <!-- Glassmorphism Container Frame -->
  <rect x="30" y="30" width="1140" height="420" rx="12" fill="#0B132B" fill-opacity="0.3" stroke="url(#glass-border)" stroke-width="1.5" />

  <!-- Animated Border Laser Lines -->
  <path class="laser-line" d="M 30 30 L 1170 30 L 1170 450 L 30 450 Z" fill="none" stroke="#38BDF8" stroke-width="2" />

  <!-- Hero Content Center -->
  <g transform="translate(600, 180)" text-anchor="middle">
    
    <!-- Animated Conlink Brand Emblem -->
    <g transform="translate(0, -75)">
      <!-- Ring 1 -->
      <circle cx="0" cy="0" r="32" fill="none" stroke="url(#conlink-grad)" stroke-width="2.5" stroke-dasharray="150 50">
        <animateTransform attributeName="transform" type="rotate" from="0" to="360" dur="12s" repeatCount="indefinite" />
      </circle>
      <!-- Ring 2 -->
      <circle cx="0" cy="0" r="22" fill="none" stroke="#00F2FE" stroke-width="1.5" stroke-dasharray="80 40">
        <animateTransform attributeName="transform" type="rotate" from="360" to="0" dur="8s" repeatCount="indefinite" />
      </circle>
      <!-- Core Node -->
      <circle cx="0" cy="0" r="8" fill="url(#conlink-grad)">
        <animate attributeName="r" values="6;9;6" dur="3s" repeatCount="indefinite" />
      </circle>
      <!-- Orbital Dots -->
      <circle cx="0" cy="-22" r="3" fill="#38BDF8">
        <animateTransform attributeName="transform" type="rotate" from="0" to="360" dur="8s" repeatCount="indefinite" />
      </circle>
    </g>

    <!-- Subtitle / Role -->
    <text y="20" class="hero-subtitle">BORIS • FULL STACK SOFTWARE ENGINEER</text>

    <!-- Main Title -->
    <text y="85" class="hero-title">Architecting Modern Web Systems</text>

    <!-- Status Badge & Description -->
    <g transform="translate(0, 130)">
      <!-- Glass Pill Base -->
      <rect x="-240" y="-18" width="480" height="36" rx="18" fill="#0F172A" fill-opacity="0.8" stroke="#334155" stroke-width="1" />
      
      <!-- Live Status Indicator -->
      <circle cx="-215" cy="0" r="4" fill="#10B981">
        <animate attributeName="opacity" values="1;0.3;1" dur="2s" repeatCount="indefinite" />
      </circle>
      <circle cx="-215" cy="0" r="8" fill="none" stroke="#10B981" stroke-width="1" opacity="0.5">
        <animate attributeName="r" values="4;12" dur="2s" repeatCount="indefinite" />
        <animate attributeName="opacity" values="0.8;0" dur="2s" repeatCount="indefinite" />
      </circle>

      <text x="-195" y="5" text-anchor="start" font-size="13" font-weight="600" fill="#E2E8F0" letter-spacing="0.5">CURRENTLY BUILDING</text>
      <text x="-35" y="5" text-anchor="start" font-size="13" font-weight="700" fill="#38BDF8" letter-spacing="0.5">CONLINK MESSENGER</text>
      <text x="125" y="5" text-anchor="start" font-size="13" font-weight="400" fill="#64748B">|</text>
      <text x="140" y="5" text-anchor="start" font-size="13" font-weight="500" fill="#94A3B8">JS • PHP • MySQL</text>
    </g>
  </g>

  <!-- Bottom Accent Tech Line -->
  <path d="M 100 410 L 1100 410" stroke="#1E293B" stroke-width="1" />
  <path d="M 500 410 L 700 410" stroke="url(#conlink-grad)" stroke-width="2">
    <animate attributeName="d" values="M 300 410 L 500 410; M 700 410 L 900 410; M 300 410 L 500 410" dur="6s" repeatCount="indefinite" />
  </path>
</svg>

<br/>

<!-- NAVIGATION MENU -->
<table border="0" width="100%" cell-spacing="0" cell-padding="0">
  <tr>
    <td align="center" style="background: #090D16; border: 1px solid #1E293B; border-radius: 30px; padding: 8px 16px;">
      <a href="#about-me"><b>ABOUT</b></a> &nbsp;•&nbsp;
      <a href="#featured-project"><b>PROJECTS</b></a> &nbsp;•&nbsp;
      <a href="#tech-stack"><b>STACK</b></a> &nbsp;•&nbsp;
      <a href="#engineering-principles"><b>PHILOSOPHY</b></a> &nbsp;•&nbsp;
      <a href="#github-analytics"><b>ANALYTICS</b></a> &nbsp;•&nbsp;
      <a href="#connect"><b>CONTACT</b></a>
    </td>
  </tr>
</table>

</div>

<br/><br/>

<!-- SECTION DIVIDER -->
<svg xmlns="http://www.w3.org/2000/svg" viewBox="0 0 1200 8" width="100%" height="8" style="display: block;">
  <defs>
    <linearGradient id="div-grad-1" x1="0%" y1="0%" x2="100%" y2="0%">
      <stop offset="0%" stop-color="#080D1A" />
      <stop offset="50%" stop-color="#38BDF8" />
      <stop offset="100%" stop-color="#080D1A" />
    </linearGradient>
  </defs>
  <rect width="1200" height="2" y="3" fill="url(#div-grad-1)" opacity="0.6" />
</svg>

<br/>

<a id="about-me"></a>
## 01. EXECUTIVE SUMMARY

<table stroke="0" width="100%" cell-padding="0" cell-spacing="0" style="border-collapse: collapse; border: none;">
<tr>
<td width="60%" valign="top" style="border: none; padding-right: 20px;">

### Engineering High-Performance Systems with Precision

I am a **Full Stack Software Engineer** specializing in building secure, resilient, and ultra-fast web applications. My methodology revolves around clean architectural patterns, robust data structures, and flawless user experiences inspired by industry-defining products like Vercel, Linear, and Apple.

My primary focus is on **Conlink Messenger**—a next-generation messaging platform engineered with a high-throughput **PHP/MySQL** backend architecture and an interactive **JavaScript** dynamic frontend.

* **Core Focus:** Full Stack Systems, Real-Time Messaging Architecture, Database Optimization
* **Primary Stack:** JavaScript (ES6+), PHP 8+, MySQL, React, RESTful APIs, Tailwind CSS
* **Design Mindset:** Ultra-minimalist UI/UX, Glassmorphism, Micro-interactions, Accessibility
* **Code Philosophy:** Strict typing, self-documenting code, zero unnecessary dependencies

</td>
<td width="40%" valign="top" style="border: none;">

```yaml
# BORIS // SYSTEM MANIFEST

developer_profile:
  alias: "BorisXQ"
  role: "Full Stack Software Engineer"
  location: "Europe / Remote"
  status: "Active Architecture & Dev"
  
core_metrics:
  code_style: "Clean / Modular / Declarative"
  architecture: "Monolithic Core / Micro Services"
  db_strategy: "Optimized Indexing / Relational Schema"
  frontend_speed: "Sub-100ms TTFB / Zero Layout Shift"

current_focus:
  project: "Conlink Messenger"
  phase: "Core Engine Optimization"
