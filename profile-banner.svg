    <radialGradient id="bgGlow2" cx="80%" cy="80%" r="50%">
        <stop offset="0%" stop-color="#10B981" stop-opacity="0.15">
            <animate attributeName="stop-color" values="#10B981;#7C3AED;#22D3EE;#10B981" dur="20s" repeatCount="indefinite" />
        </stop>
        <stop offset="100%" stop-color="#030712" stop-opacity="0" />
    </radialGradient>

    <!-- Accent Gradient for Main Title -->
    <linearGradient id="accentGradient" x1="0%" y1="0%" x2="100%" y2="100%">
        <stop offset="0%" stop-color="#7C3AED">
            <animate attributeName="stop-color" values="#7C3AED;#22D3EE;#10B981;#7C3AED" dur="8s" repeatCount="indefinite" />
        </stop>
        <stop offset="50%" stop-color="#22D3EE">
            <animate attributeName="stop-color" values="#22D3EE;#10B981;#7C3AED;#22D3EE" dur="8s" repeatCount="indefinite" />
        </stop>
        <stop offset="100%" stop-color="#10B981">
            <animate attributeName="stop-color" values="#10B981;#7C3AED;#22D3EE;#10B981" dur="8s" repeatCount="indefinite" />
        </stop>
    </linearGradient>

    <!-- ASCII Terminal Gradient -->
    <linearGradient id="asciiGradient" x1="0%" y1="0%" x2="0%" y2="100%">
        <stop offset="0%" stop-color="#22D3EE" />
        <stop offset="50%" stop-color="#10B981" />
        <stop offset="100%" stop-color="#7C3AED" />
    </linearGradient>

    <!-- Glass Panel Borders with Shimmer -->
    <linearGradient id="glassBorder" x1="0%" y1="0%" x2="100%" y2="100%">
        <stop offset="0%" stop-color="rgba(255,255,255,0.2)">
            <animate attributeName="stop-color" values="rgba(255,255,255,0.2);rgba(255,255,255,0.02);rgba(255,255,255,0.2)" dur="4s" repeatCount="indefinite"/>
        </stop>
        <stop offset="50%" stop-color="rgba(255,255,255,0.02)" />
        <stop offset="100%" stop-color="rgba(255,255,255,0.1)" />
    </linearGradient>

    <!-- STREAMING_CHUNK:Configuring clip paths, patterns, and filters... -->
    <!-- Clip Paths -->
    <clipPath id="leftPanelClip">
        <rect x="30" y="30" width="420" height="550" rx="24" />
    </clipPath>
    
    <clipPath id="typingMask">
        <rect x="510" y="190" width="0" height="30">
            <animate attributeName="width" values="0; 400; 400; 0; 0" keyTimes="0; 0.2; 0.8; 0.9; 1" dur="4s" repeatCount="indefinite" />
        </rect>
    </clipPath>

    <!-- Patterns -->
    <pattern id="noise" width="100" height="100" patternUnits="userSpaceOnUse">
        <image href="data:image/svg+xml,%3Csvg viewBox='0 0 200 200' xmlns='http://www.w3.org/2000/svg'%3E%3Cfilter id='noiseFilter'%3E%3CfeTurbulence type='fractalNoise' baseFrequency='0.85' numOctaves='3' stitchTiles='stitch'/%3E%3C/filter%3E%3Crect width='100%25' height='100%25' filter='url(%23noiseFilter)' opacity='0.08'/%3E%3C/svg%3E" width="100" height="100" />
    </pattern>
    
    <pattern id="dots" width="30" height="30" patternUnits="userSpaceOnUse">
        <circle cx="15" cy="15" r="1" fill="rgba(255,255,255,0.05)" />
    </pattern>

    <!-- Glow Filter -->
    <filter id="glow" x="-20%" y="-20%" width="140%" height="140%">
        <feGaussianBlur stdDeviation="8" result="blur" />
        <feComposite in="SourceGraphic" in2="blur" operator="over" />
    </filter>
</defs>

<!-- STREAMING_CHUNK:Rendering background and ambient lighting layers... -->
<!-- Base Background -->
<rect width="1180" height="610" fill="#030712" />
<rect width="1180" height="610" fill="url(#bgGlow1)" />
<rect width="1180" height="610" fill="url(#bgGlow2)" />
<rect width="1180" height="610" fill="url(#dots)" />
<rect width="1180" height="610" fill="url(#noise)" style="pointer-events: none;" />

<!-- Animated Floating Particles -->
<g fill="#22D3EE" opacity="0.3" filter="url(#glow)">
    <circle cx="200" cy="500" r="2"><animateMotion path="M0,0 Q50,-50 100,0 T200,0 T0,0" dur="15s" repeatCount="indefinite"/></circle>
    <circle cx="800" cy="100" r="1.5"><animateMotion path="M0,0 Q-50,50 -100,0 T-200,0 T0,0" dur="25s" repeatCount="indefinite"/></circle>
    <circle cx="600" cy="550" r="2.5"><animateMotion path="M0,0 Q30,-70 60,0 T120,0 T0,0" dur="18s" repeatCount="indefinite"/></circle>
    <circle cx="100" cy="150" r="1.5"><animateMotion path="M0,0 Q60,60 120,0 T240,0 T0,0" dur="22s" repeatCount="indefinite"/></circle>
</g>

<!-- Global Font Configuration -->
<g font-family="system-ui, -apple-system, BlinkMacSystemFont, 'Segoe UI', Roboto, 'Helvetica Neue', sans-serif">
    
    <!-- STREAMING_CHUNK:Building Left Panel (ASCII Portrait & Cyber Elements)... -->
    <!-- LEFT PANEL: ASCII Art / Terminal -->
    <g transform="translate(0, 0)">
        <rect x="30" y="30" width="420" height="550" rx="24" fill="#0F172A" fill-opacity="0.6" stroke="url(#glassBorder)" stroke-width="1" />
        
        <g clip-path="url(#leftPanelClip)">
            <!-- Floating animation for ASCII -->
            <g>
                <animateTransform attributeName="transform" type="translate" values="0 0; 0 -10; 0 0" dur="8s" repeatCount="indefinite" />
                
                <text x="55" y="80" fill="#94A3B8" font-size="12" font-family="monospace" letter-spacing="1">SYSTEM BOOT...</text>
                <text x="55" y="100" fill="#94A3B8" font-size="12" font-family="monospace" letter-spacing="1">KERNEL V. 9.1.4</text>

                <!-- The Core ASCII Graphic -->
                <g fill="url(#asciiGradient)" font-size="14" font-family="monospace" letter-spacing="1" font-weight="bold">
                    <text x="55" y="140">      ___       __  __ </text>
                    <text x="55" y="158">     /   |     / / / / </text>
                    <text x="55" y="176">    / /| |    / /_/ /  </text>
                    <text x="55" y="194">   / ___ |   / __  /   </text>
                    <text x="55" y="212">  /_/  |_|  /_/ /_/    </text>
                    
                    <text x="55" y="248">[ SYNAPSE NEURAL CORE ]</text>
                    <text x="55" y="266">[ STATUS: ACTIVATED ]</text>
                </g>
                
                <g fill="#F8FAFC" font-size="13" font-family="monospace" letter-spacing="0.5">
                    <text x="55" y="310">&gt; INIT: ML PIPELINE...</text>
                    <text x="55" y="330">&gt; LOAD: TENSORFLOW 2.x</text>
                    <text x="55" y="350">&gt; LOAD: PYTORCH 2.0</text>
                    <text x="55" y="370">&gt; SYNC: GCP ARCADE '26</text>
                    <text x="55" y="390">&gt; CALC: NEURAL WEIGHTS</text>
                    <text x="55" y="410">&gt; OPTIMIZE: LEETCODE</text>
                </g>

                <text x="55" y="460" fill="#10B981" font-size="13" font-family="monospace" letter-spacing="2">[████████████████████] 100%</text>

                <text x="55" y="500" fill="#94A3B8" font-size="12" font-family="monospace" letter-spacing="1">CONNECTION ESTABLISHED.</text>
                <text x="55" y="520" fill="#F8FAFC" font-size="12" font-family="monospace" letter-spacing="1">READY FOR INPUT<tspan fill="#22D3EE"><animate attributeName="opacity" values="1;0;1" dur="1s" repeatCount="indefinite"/>_</tspan></text>
            </g>
            
            <!-- Terminal Scanline Effect -->
            <rect x="30" y="30" width="420" height="3" fill="#22D3EE" opacity="0.4" filter="url(#glow)">
                <animate attributeName="y" values="30; 580; 30" dur="6s" repeatCount="indefinite" />
            </rect>
        </g>
    </g>

    <!-- STREAMING_CHUNK:Building Right Panel (Glassmorphism UI, Header & Typography)... -->
    <!-- RIGHT PANEL: Main Profile Information -->
    <g transform="translate(0, 0)">
        <rect x="470" y="30" width="680" height="550" rx="24" fill="#0F172A" fill-opacity="0.6" stroke="url(#glassBorder)" stroke-width="1" />
        
        <!-- Social Navigation / Top Right -->
        <g fill="#94A3B8" transform="translate(0, 50)">
            <!-- GitHub -->
            <g transform="translate(940, 0)"><path d="M12 2C6.477 2 2 6.484 2 12.017c0 4.425 2.865 8.18 6.839 9.504.5.092.682-.217.682-.483 0-.237-.008-.868-.013-1.703-2.782.605-3.369-1.343-3.369-1.343-.454-1.158-1.11-1.466-1.11-1.466-.908-.62.069-.608.069-.608 1.003.07 1.531 1.032 1.531 1.032.892 1.53 2.341 1.088 2.91.832.092-.647.35-1.088.636-1.338-2.22-.253-4.555-1.113-4.555-4.951 0-1.093.39-1.988 1.029-2.688-.103-.253-.446-1.272.098-2.65 0 0 .84-.27 2.75 1.026A9.564 9.564 0 0112 6.844c.85.004 1.705.115 2.504.337 1.909-1.296 2.747-1.027 2.747-1.027.546 1.379.202 2.398.1 2.651.64.7 1.028 1.595 1.028 2.688 0 3.848-2.339 4.695-4.566 4.943.359.309.678.92.678 1.855 0 1.338-.012 2.419-.012 2.747 0 .268.18.58.688.482A10.019 10.019 0 0022 12.017C22 6.484 17.522 2 12 2z"/></g>
            <!-- LinkedIn -->
            <g transform="translate(980, 0)"><path d="M20.447 20.452h-3.554v-5.569c0-1.328-.027-3.037-1.852-3.037-1.853 0-2.136 1.445-2.136 2.939v5.667H9.351V9h3.414v1.561h.046c.477-.9 1.637-1.85 3.37-1.85 3.601 0 4.267 2.37 4.267 5.455v6.286zM5.337 7.433c-1.144 0-2.063-.926-2.063-2.065 0-1.138.92-2.063 2.063-2.063 1.14 0 2.064.925 2.064 2.063 0 1.139-.925 2.065-2.064 2.065zm1.782 13.019H3.555V9h3.564v11.452zM22.225 0H1.771C.792 0 0 .774 0 1.729v20.542C0 23.227.792 24 1.771 24h20.451C23.2 24 24 23.227 24 22.271V1.729C24 .774 23.2 0 22.222 0h.003z"/></g>
            <!-- LeetCode -->
            <g transform="translate(1020, 0)"><path d="M16.1 22.21l-5.41 1.44c-2.4.64-4.88-.7-5.61-3.06L3.9 16.27c-.73-2.36.56-4.94 2.96-5.58l5.41-1.44c2.4-.64 4.88.7 5.61 3.06l1.18 4.32c.73 2.36-.56 4.94-2.96 5.58zm-1.83-8.85l-4.54 1.2c-1.1.29-1.74 1.48-1.41 2.56l.82 3c.33 1.08 1.47 1.7 2.57 1.41l4.54-1.2c1.1-.29 1.74-1.48 1.41-2.56l-.82-3c-.33-1.08-1.47-1.7-2.57-1.41zM20.25 5.53L15.34 1.2c-1.39-1.22-3.48-1.09-4.72.29l-6.17 6.84c-1.24 1.38-1.11 3.49.29 4.7l4.9 4.33c1.39 1.22 3.48 1.09 4.72-.29l6.17-6.84c1.24-1.38 1.11-3.49-.28-4.7z"/></g>
            <!-- Portfolio -->
            <g transform="translate(1060, 0)"><path d="M12 2C6.48 2 2 6.48 2 12s4.48 10 10 10 10-4.48 10-10S17.52 2 12 2zm1 15h-2v-2h2v2zm0-4h-2V7h2v6z"/></g>
            <!-- Email -->
            <g transform="translate(1100, 0)"><path d="M20 4H4c-1.1 0-1.99.9-1.99 2L2 18c0 1.1.9 2 2 2h16c1.1 0 2-.9 2-2V6c0-1.1-.9-2-2-2zm0 4l-8 5-8-5V6l8 5 8-5v2z"/></g>
        </g>

        <!-- Greeting Text -->
        <text x="510" y="80" fill="#94A3B8" font-size="18" font-weight="500">Hi 👋 I'm</text>
        <text x="510" y="115" fill="#F8FAFC" font-size="28" font-weight="600">Rohit Hanuman Sai</text>
        
        <!-- Animated Gradient Last Name -->
        <text x="510" y="165" fill="url(#accentGradient)" font-size="46" font-weight="800" letter-spacing="1">PUTTAGUNTA</text>

        <!-- STREAMING_CHUNK:Injecting Animated Typing Effect engine... -->
        <!-- Typing Effect Phrase Rotator -->
        <g transform="translate(0, 0)" font-size="20" font-weight="600" fill="#22D3EE">
            <!-- We use 8 phrases, total duration 32s (4s each). -->
            <g clip-path="url(#typingMask)">
                <text x="510" y="210" opacity="0"><animate attributeName="opacity" values="1;1;0;0;0;0;0;0;0" keyTimes="0; 0.124; 0.125; 0.25; 0.375; 0.5; 0.625; 0.75; 1" dur="32s" repeatCount="indefinite" />AI Engineer</text>
                <text x="510" y="210" opacity="0"><animate attributeName="opacity" values="0;0;1;1;0;0;0;0;0" keyTimes="0; 0.124; 0.125; 0.249; 0.25; 0.375; 0.5; 0.625; 1" dur="32s" repeatCount="indefinite" />Machine Learning Enthusiast</text>
                <text x="510" y="210" opacity="0"><animate attributeName="opacity" values="0;0;0;0;1;1;0;0;0" keyTimes="0; 0.249; 0.25; 0.374; 0.375; 0.499; 0.5; 0.75; 1" dur="32s" repeatCount="indefinite" />Data Science Undergraduate</text>
                <text x="510" y="210" opacity="0"><animate attributeName="opacity" values="0;0;0;0;0;0;1;1;0" keyTimes="0; 0.374; 0.375; 0.499; 0.5; 0.624; 0.625; 0.75; 1" dur="32s" repeatCount="indefinite" />Full Stack Developer</text>
                <text x="510" y="210" opacity="0"><animate attributeName="opacity" values="0;0;0;0;0;0;0;0;1" keyTimes="0; 0.499; 0.5; 0.624; 0.625; 0.749; 0.75; 0.875; 1" dur="32s" repeatCount="indefinite" />Cloud Computing Enthusiast</text>
                <text x="510" y="210" opacity="0"><animate attributeName="opacity" values="1;0;0;0;0;0;0;0;0" keyTimes="0; 0.624; 0.625; 0.749; 0.75; 0.874; 0.875; 0.999; 1" dur="32s" repeatCount="indefinite" />LeetCode Knight</text>
                <text x="510" y="210" opacity="0"><animate attributeName="opacity" values="0;1;0;0;0;0;0;0;0" keyTimes="0; 0.749; 0.75; 0.874; 0.875; 0.999; 1; 1; 1" dur="32s" repeatCount="indefinite" />Open Source Learner</text>
                <text x="510" y="210" opacity="0"><animate attributeName="opacity" values="0;0;1;0;0;0;0;0;0" keyTimes="0; 0.874; 0.875; 0.999; 1; 1; 1; 1; 1" dur="32s" repeatCount="indefinite" />Building Intelligent Systems</text>
            </g>
            <!-- Blinking cursor matching the text -->
            <text x="510" y="210" fill="#10B981"><animate attributeName="x" values="615; 765; 755; 705; 755; 660; 695; 760" keyTimes="0; 0.125; 0.25; 0.375; 0.5; 0.625; 0.75; 0.875" dur="32s" calcMode="discrete" repeatCount="indefinite"/><animate attributeName="opacity" values="1;0;1" dur="0.8s" repeatCount="indefinite"/>_</text>
        </g>

        <!-- STREAMING_CHUNK:Structuring Information Grid... -->
        <!-- Information Rows -->
        <g font-size="13" font-weight="500" fill="#94A3B8">
            <!-- Column 1 -->
            <g transform="translate(510, 260)">
                <text x="25" y="0">📍 Vijayawada, Andhra Pradesh, India</text>
                <text x="25" y="30">🏫 PVP Siddhartha Institute of Technology</text>
                <text x="25" y="60">☁️ Google Cloud Arcade Facilitator 2026</text>
                <text x="25" y="90">🧠 LeetCode Knight | 290+ Solved</text>
            </g>
            <!-- Column 2 -->
            <g transform="translate(830, 260)">
                <text x="25" y="0">🎓 B.Tech Computer Science (DS)</text>
                <text x="25" y="30">💼 AI • ML • Full Stack</text>
                <text x="25" y="60">🏆 Smart Intv. — Top 3 Class</text>
                <text x="25" y="90">🌐 Portfolio | 📧 Email</text>
            </g>
        </g>

        <!-- STREAMING_CHUNK:Rendering Premium Glass Skills Pills... -->
        <!-- Skills Section -->
        <text x="510" y="380" fill="#F8FAFC" font-size="14" font-weight="600" letter-spacing="1">SKILLS &amp; TECHNOLOGIES</text>
        
        <g font-size="12" font-weight="500" fill="#E2E8F0">
            <!-- Row 1 -->
            <g transform="translate(510, 400)">
                <rect x="0" y="0" width="60" height="24" rx="6" fill="rgba(255,255,255,0.05)" stroke="rgba(255,255,255,0.1)"/><text x="30" y="16" text-anchor="middle">Python</text>
                <rect x="68" y="0" width="50" height="24" rx="6" fill="rgba(255,255,255,0.05)" stroke="rgba(255,255,255,0.1)"/><text x="93" y="16" text-anchor="middle">Java</text>
                <rect x="126" y="0" width="65" height="24" rx="6" fill="rgba(255,255,255,0.05)" stroke="rgba(255,255,255,0.1)"/><text x="158.5" y="16" text-anchor="middle">FastAPI</text>
                <rect x="199" y="0" width="60" height="24" rx="6" fill="rgba(255,255,255,0.05)" stroke="rgba(255,255,255,0.1)"/><text x="229" y="16" text-anchor="middle">React</text>
                <rect x="267" y="0" width="65" height="24" rx="6" fill="rgba(255,255,255,0.05)" stroke="rgba(255,255,255,0.1)"/><text x="299.5" y="16" text-anchor="middle">Next.js</text>
                <rect x="340" y="0" width="65" height="24" rx="6" fill="rgba(255,255,255,0.05)" stroke="rgba(255,255,255,0.1)"/><text x="372.5" y="16" text-anchor="middle">Node.js</text>
                <rect x="413" y="0" width="85" height="24" rx="6" fill="rgba(255,255,255,0.05)" stroke="rgba(255,255,255,0.1)"/><text x="455.5" y="16" text-anchor="middle">TypeScript</text>
                <rect x="506" y="0" width="65" height="24" rx="6" fill="rgba(255,255,255,0.05)" stroke="rgba(255,255,255,0.1)"/><text x="538.5" y="16" text-anchor="middle">Docker</text>
            </g>
            <!-- Row 2 -->
            <g transform="translate(510, 432)">
                <rect x="0" y="0" width="90" height="24" rx="6" fill="rgba(255,255,255,0.05)" stroke="rgba(255,255,255,0.1)"/><text x="45" y="16" text-anchor="middle">Kubernetes</text>
                <rect x="98" y="0" width="90" height="24" rx="6" fill="rgba(255,255,255,0.05)" stroke="rgba(255,255,255,0.1)"/><text x="143" y="16" text-anchor="middle">PostgreSQL</text>
                <rect x="196" y="0" width="80" height="24" rx="6" fill="rgba(255,255,255,0.05)" stroke="rgba(255,255,255,0.1)"/><text x="236" y="16" text-anchor="middle">MongoDB</text>
                <rect x="284" y="0" width="45" height="24" rx="6" fill="rgba(255,255,255,0.05)" stroke="rgba(255,255,255,0.1)"/><text x="306.5" y="16" text-anchor="middle">Git</text>
                <rect x="337" y="0" width="60" height="24" rx="6" fill="rgba(255,255,255,0.05)" stroke="rgba(255,255,255,0.1)"/><text x="367" y="16" text-anchor="middle">GitHub</text>
                <rect x="405" y="0" width="95" height="24" rx="6" fill="rgba(255,255,255,0.05)" stroke="rgba(255,255,255,0.1)"/><text x="452.5" y="16" text-anchor="middle">Google Cloud</text>
                <rect x="508" y="0" width="85" height="24" rx="6" fill="rgba(255,255,255,0.05)" stroke="rgba(255,255,255,0.1)"/><text x="550.5" y="16" text-anchor="middle">TensorFlow</text>
            </g>
            <!-- Row 3 -->
            <g transform="translate(510, 464)">
                <rect x="0" y="0" width="75" height="24" rx="6" fill="rgba(255,255,255,0.05)" stroke="rgba(255,255,255,0.1)"/><text x="37.5" y="16" text-anchor="middle">PyTorch</text>
                <rect x="83" y="0" width="125" height="24" rx="6" fill="rgba(255,255,255,0.05)" stroke="rgba(255,255,255,0.1)"/><text x="145.5" y="16" text-anchor="middle">Machine Learning</text>
                <rect x="216" y="0" width="135" height="24" rx="6" fill="rgba(255,255,255,0.05)" stroke="rgba(255,255,255,0.1)"/><text x="283.5" y="16" text-anchor="middle">Artificial Intelligence</text>
                <rect x="359" y="0" width="95" height="24" rx="6" fill="rgba(255,255,255,0.05)" stroke="rgba(255,255,255,0.1)"/><text x="406.5" y="16" text-anchor="middle">Data Science</text>
                <rect x="462" y="0" width="55" height="24" rx="6" fill="rgba(255,255,255,0.05)" stroke="rgba(255,255,255,0.1)"/><text x="489.5" y="16" text-anchor="middle">Linux</text>
            </g>
        </g>

        <!-- STREAMING_CHUNK:Finalizing layout with Achievements Cards... -->
        <!-- Achievements & Projects -->
        <text x="510" y="525" fill="#F8FAFC" font-size="14" font-weight="600" letter-spacing="1">ACHIEVEMENTS &amp; PROJECTS</text>
        
        <g font-size="12" font-weight="600" fill="#38BDF8">
            <!-- Card 1 -->
            <g transform="translate(510, 545)">
                <rect x="0" y="0" width="135" height="35" rx="8" fill="rgba(16,185,129,0.05)" stroke="rgba(16,185,129,0.2)"/>
                <text x="67.5" y="22" text-anchor="middle" fill="#10B981">🏆 LeetCode Knight</text>
            </g>
            <!-- Card 2 -->
            <g transform="translate(655, 545)">
                <rect x="0" y="0" width="140" height="35" rx="8" fill="rgba(124,58,237,0.05)" stroke="rgba(124,58,237,0.2)"/>
                <text x="70" y="22" text-anchor="middle" fill="#A78BFA">🥉 Smart Interviews</text>
            </g>
            <!-- Card 3 -->
            <g transform="translate(805, 545)">
                <rect x="0" y="0" width="145" height="35" rx="8" fill="rgba(34,211,238,0.05)" stroke="rgba(34,211,238,0.2)"/>
                <text x="72.5" y="22" text-anchor="middle" fill="#22D3EE">☁️ GCP Facilitator</text>
            </g>
            <!-- Card 4 -->
            <g transform="translate(960, 545)">
                <rect x="0" y="0" width="120" height="35" rx="8" fill="rgba(248,250,252,0.05)" stroke="rgba(248,250,252,0.2)"/>
                <text x="60" y="22" text-anchor="middle" fill="#F8FAFC">🤖 SYNAPSE AI</text>
            </g>
        </g>
    </g>
</g>
