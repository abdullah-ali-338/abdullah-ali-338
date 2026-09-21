<!DOCTYPE html>
<html lang="en" class="scroll-smooth">
<head>
<meta charset="UTF-8">
<meta name="viewport" content="width=device-width, initial-scale=1.0">
<title>Abdullah Ali - Portfolio</title>
<script src="https://cdn.tailwindcss.com"></script>
<link href="https://fonts.googleapis.com/css2?family=Helvetica+Neue:wght@400;500;700&family=JetBrains+Mono:wght@400;700&display=swap" rel="stylesheet">
<style>
    :root {
        --bg: #111111;
        --fg: #E8E8E8;
        --border: #262626;
        --accent: #FFFFFF;
    }
    body {
        background-color: var(--bg);
        color: var(--fg);
        font-family: 'Helvetica Neue', Helvetica, Arial, sans-serif;
        overflow-x: hidden;
    }
    .font-mono { font-family: 'JetBrains Mono', monospace; }
    
    .frame {
        position: fixed;
        top: 0; left: 0; right: 0; bottom: 0;
        pointer-events: none;
        z-index: 100;
        border: 1px solid transparent;
    }
    .frame__mark {
        position: absolute;
        width: 16px; height: 16px;
        border-color: var(--border);
        border-style: solid;
    }
    .frame__mark--tl { top: 12px; left: 12px; border-width: 1px 0 0 1px; }
    .frame__mark--tr { top: 12px; right: 12px; border-width: 1px 1px 0 0; }
    .frame__mark--bl { bottom: 12px; left: 12px; border-width: 0 0 1px 1px; }
    .frame__mark--br { bottom: 12px; right: 12px; border-width: 0 1px 1px 0; }
    .frame__edge {
        position: absolute;
        font-family: 'JetBrains Mono', monospace;
        font-size: 0.6rem;
        color: #555555;
        letter-spacing: 0.12em;
    }
    .frame__edge--left { top: 50%; left: 14px; transform: translateY(-50%) rotate(-90deg); transform-origin: left top; }
    .frame__edge--right { top: 50%; right: 14px; transform: translateY(-50%) rotate(90deg); transform-origin: right top; }

    .meta-label {
        font-family: 'JetBrains Mono', monospace;
        font-size: 0.65rem;
        text-transform: uppercase;
        color: #737373;
        display: block;
        margin-bottom: 0.25rem;
    }
    .meta-value {
        font-size: 0.85rem;
        font-weight: 500;
    }

    .hairline-b { border-bottom: 1px solid var(--border); }
    .hairline-t { border-top: 1px solid var(--border); }
    .hairline-l { border-left: 1px solid var(--border); }
    .hairline-r { border-right: 1px solid var(--border); }
    .hairline-all { border: 1px solid var(--border); }

    .invert-section {
        background-color: var(--fg);
        color: var(--bg);
    }
    .invert-section .meta-label { color: #555555; }
    .invert-section .hairline-b, 
    .invert-section .hairline-t,
    .invert-section .hairline-l { border-color: #D4D4D4; }
</style>
</head>
<body class="p-4 md:p-12 relative selection:bg-white selection:text-black">

    <div class="frame hidden md:block">
        <span class="frame__mark frame__mark--tl"></span>
        <span class="frame__mark frame__mark--tr"></span>
        <span class="frame__mark frame__mark--bl"></span>
        <span class="frame__mark frame__mark--br"></span>
        <span class="frame__edge frame__edge--left">PORTFOLIO&nbsp;-&nbsp;V.01</span>
        <span class="frame__edge frame__edge--right">OBJ.ABDULLAH_ALI</span>
    </div>

    <!-- NAV -->
    <header class="flex justify-between items-center hairline-b pb-4 mb-12">
        <a href="#" class="font-bold tracking-tight text-lg uppercase">Abdullah Ali</a>
        <nav class="hidden md:flex gap-8 font-mono text-xs uppercase tracking-wider text-neutral-400">
            <a href="#about" class="hover:text-white transition-colors">Profile</a>
            <a href="#work" class="hover:text-white transition-colors">Catalog</a>
            <a href="#experience" class="hover:text-white transition-colors">Timeline</a>
        </nav>
        <a href="#contact" class="font-mono text-xs uppercase hover:text-white transition-colors">Contact</a>
    </header>

    <!-- HERO META -->
    <section class="grid grid-cols-2 md:grid-cols-4 gap-6 mb-16 hairline-b pb-12">
        <div>
            <span class="meta-label">Location</span>
            <span class="meta-value">Lahore, Pakistan</span>
        </div>
        <div>
            <span class="meta-label">Discipline</span>
            <span class="meta-value">Backend / Systems</span>
        </div>
        <div>
            <span class="meta-label">Status</span>
            <span class="meta-value">Available</span>
        </div>
        <div>
            <span class="meta-label">Index</span>
            <span class="meta-value">01_2026</span>
        </div>
    </section>

    <!-- HERO TITLE -->
    <section class="mb-16">
        <h1 class="text-5xl md:text-8xl font-bold uppercase tracking-tighter leading-[0.9] mb-6">
            Abdullah <br> Ali <span class="text-3xl md:text-5xl text-neutral-600 font-mono font-normal tracking-normal">• 01</span>
        </h1>
        <p class="text-xl md:text-2xl text-neutral-400 max-w-2xl font-light">
            Backend Engineering and System architecture, building high-performance APIs and tools, quietly.
        </p>
    </section>

    <!-- SPEC STRIP -->
    <nav class="grid grid-cols-2 md:grid-cols-4 hairline-t hairline-b divide-x divide-[#262626] font-mono text-xs uppercase tracking-widest mb-24">
        <a href="#about" class="p-4 hover:bg-[#161616] transition-colors flex flex-col"><span class="text-neutral-500 mb-1">01</span>Profile</a>
        <a href="#work" class="p-4 hover:bg-[#161616] transition-colors flex flex-col"><span class="text-neutral-500 mb-1">02</span>Selected Work</a>
        <a href="#experience" class="p-4 hover:bg-[#161616] transition-colors flex flex-col"><span class="text-neutral-500 mb-1">03</span>Experience</a>
        <a href="#contact" class="p-4 hover:bg-[#161616] transition-colors flex flex-col"><span class="text-neutral-500 mb-1">04</span>Contact</a>
    </nav>

    <!-- ABOUT -->
    <section id="about" class="mb-24 md:flex gap-12">
        <div class="md:w-1/3 mb-8 md:mb-0">
            <span class="meta-label">01 / Profile</span>
        </div>
        <div class="md:w-2/3">
            <h2 class="text-3xl md:text-5xl font-bold leading-tight mb-8">
                Building scalable<br>backend systems and<br>low-latency architectures.
            </h2>
            <p class="text-lg text-neutral-400 leading-relaxed mb-12 max-w-2xl">
                I am a backend engineer focusing on Python, API design, and deterministic workflows. I construct concise, purposeful software systems rather than bloated generalities.
            </p>
            <div class="grid grid-cols-2 gap-8 font-mono text-sm hairline-t pt-8">
                <div>
                    <span class="meta-label">Based</span>
                    <span class="text-white">Pakistan</span>
                </div>
                <div>
                    <span class="meta-label">Focus</span>
                    <span class="text-white">Backend Engineering</span>
                </div>
                <div>
                    <span class="meta-label">Practice</span>
                    <span class="text-white">Python, Flask, C++</span>
                </div>
                <div>
                    <span class="meta-label">Availability</span>
                    <span class="text-white">Open to Roles</span>
                </div>
            </div>
        </div>
    </section>

    <!-- WORK / CATALOG -->
    <section id="work" class="mb-24">
        <div class="mb-12 hairline-b pb-4">
            <span class="meta-label">02 / Selected Work</span>
            <h2 class="text-4xl font-bold uppercase tracking-tight">Catalog</h2>
        </div>

        <div class="grid gap-16">
            <!-- Project 1 -->
            <article class="grid md:grid-cols-12 gap-8 items-start hairline-b pb-12">
                <div class="md:col-span-5 bg-[#141414] aspect-video md:aspect-square flex items-center justify-center p-8 hairline-all relative">
                    <span class="absolute top-3 left-3 meta-label">FIG. 01</span>
                    <span class="font-mono text-neutral-500 text-lg tracking-wider">WIDGET_AI</span>
                </div>
                <div class="md:col-span-7 flex flex-col justify-center h-full">
                    <span class="font-mono text-xs text-neutral-500 mb-2">01</span>
                    <h3 class="text-3xl font-bold mb-4">Widget AI</h3>
                    <p class="text-neutral-400 text-base mb-6 leading-relaxed">
                        A mobile-first conversational AI interface. Engineered sub-second response streaming using Groq LPUs and Python/Flask with dynamic visualViewport handling.
                    </p>
                    <div class="flex flex-wrap gap-4 font-mono text-xs uppercase text-neutral-500 mb-6">
                        <span>Python</span><span>Flask</span><span>Groq</span><span>JavaScript</span>
                    </div>
                    <div class="flex gap-4">
                        <a href="https://widget-ai.duckdns.org" target="_blank" class="hairline-all px-4 py-2 text-xs font-mono uppercase hover:bg-white hover:text-black transition-colors">Live Demo</a>
                        <a href="https://github.com/abdullah-ali-338/widget-ai" target="_blank" class="hairline-all px-4 py-2 text-xs font-mono uppercase hover:bg-white hover:text-black transition-colors">Source</a>
                    </div>
                </div>
            </article>

            <!-- Project 2 -->
            <article class="grid md:grid-cols-12 gap-8 items-start hairline-b pb-12">
                <div class="md:col-span-5 bg-[#141414] aspect-video md:aspect-square flex items-center justify-center p-8 hairline-all relative">
                    <span class="absolute top-3 left-3 meta-label">FIG. 02</span>
                    <span class="font-mono text-neutral-500 text-lg tracking-wider">C++_ENGINE</span>
                </div>
                <div class="md:col-span-7 flex flex-col justify-center h-full">
                    <span class="font-mono text-xs text-neutral-500 mb-2">02</span>
                    <h3 class="text-3xl font-bold mb-4">Terminal Hangman Engine</h3>
                    <p class="text-neutral-400 text-base mb-6 leading-relaxed">
                        A modular 250+ LOC C++ terminal engine featuring 7 progressive ASCII lifecycle states and an fstream I/O pipeline for persistent state tracking.
                    </p>
                    <div class="flex flex-wrap gap-4 font-mono text-xs uppercase text-neutral-500 mb-6">
                        <span>C++</span><span>Procedural</span><span>fstream</span>
                    </div>
                    <div>
                        <a href="https://github.com/abdullah-ali-338/hangman-engine-cpp" target="_blank" class="hairline-all px-4 py-2 text-xs font-mono uppercase hover:bg-white hover:text-black transition-colors">Source</a>
                    </div>
                </div>
            </article>

            <!-- Project 3 -->
            <article class="grid md:grid-cols-12 gap-8 items-start hairline-b pb-12">
                <div class="md:col-span-5 bg-[#141414] aspect-video md:aspect-square flex items-center justify-center p-8 hairline-all relative">
                    <span class="absolute top-3 left-3 meta-label">FIG. 03</span>
                    <span class="font-mono text-neutral-500 text-lg tracking-wider">OS_LOGGER</span>
                </div>
                <div class="md:col-span-7 flex flex-col justify-center h-full">
                    <span class="font-mono text-xs text-neutral-500 mb-2">03</span>
                    <h3 class="text-3xl font-bold mb-4">Automated File Organizer</h3>
                    <p class="text-neutral-400 text-base mb-6 leading-relaxed">
                        A Python automation tool for sorting unstructured directories with structured logging and deterministic path collision handling.
                    </p>
                    <div class="flex flex-wrap gap-4 font-mono text-xs uppercase text-neutral-500 mb-6">
                        <span>Python</span><span>Automation</span><span>Logging</span>
                    </div>
                    <div>
                        <a href="https://github.com/abdullah-ali-338/automated-file-organizer-python" target="_blank" class="hairline-all px-4 py-2 text-xs font-mono uppercase hover:bg-white hover:text-black transition-colors">Source</a>
                    </div>
                </div>
            </article>
        </div>
    </section>

    <!-- TECHNICAL STACK -->
    <section class="mb-24">
        <div class="mb-8 hairline-b pb-4">
            <span class="meta-label">Index / Technical</span>
            <h2 class="text-4xl font-bold uppercase tracking-tight">Stack</h2>
        </div>
        <ul class="grid grid-cols-2 md:grid-cols-4 gap-y-4 font-mono text-xs uppercase tracking-wider text-neutral-300">
            <li>Python Ecosystem</li>
            <li>Flask Framework</li>
            <li>RESTful APIs</li>
            <li>C &amp; C++</li>
            <li>File Streams &amp; Memory</li>
            <li>JavaScript</li>
            <li>Git &amp; GitHub</li>
            <li>Render Platform</li>
        </ul>
    </section>

    <!-- EXPERIENCE / TIMELINE -->
    <section id="experience" class="mb-24">
        <div class="mb-12 hairline-b pb-4">
            <span class="meta-label">03 / Experience</span>
            <h2 class="text-4xl font-bold uppercase tracking-tight">Timeline</h2>
        </div>
        <div class="hairline-l ml-2 space-y-12">
            <div class="pl-8 relative">
                <span class="font-mono text-xs text-neutral-500 block mb-1">2026 — Present</span>
                <h3 class="text-xl font-bold mb-1">Backend Engineering Intern</h3>
                <p class="text-sm text-neutral-400 mb-2">DevConnect (Germany) — Remote</p>
                <p class="text-sm text-neutral-400 font-light">Engineered backend microservices and server logic with Python. Structured REST contracts and managed Git routines.</p>
            </div>
            <div class="pl-8 relative">
                <span class="font-mono text-xs text-neutral-500 block mb-1">2025 — 2029</span>
                <h3 class="text-xl font-bold mb-1">BS Computer Science</h3>
                <p class="text-sm text-neutral-400 mb-2">UMT Lahore</p>
                <p class="text-sm text-neutral-400 font-light">Procedural system design, low-level logic, and algorithmic efficiency.</p>
            </div>
        </div>
    </section>

    <!-- CONTACT (INVERTED) -->
    <section id="contact" class="invert-section -mx-4 md:-mx-12 -mb-4 md:-mb-12 p-8 md:p-16 hairline-t">
        <span class="meta-label mb-8">04 / Contact</span>
        <h2 class="text-5xl md:text-7xl font-bold leading-[0.9] mb-12 tracking-tighter">
            Let’s build<br>something<br>useful.
        </h2>
        
        <div class="grid md:grid-cols-3 gap-6 hairline-t hairline-b py-8 mb-12 font-mono text-xs uppercase tracking-wider">
            <a href="mailto:abdullahhh33846@gmail.com" class="group flex flex-col">
                <span class="meta-label">Email</span>
                <span class="group-hover:underline font-bold text-sm lowercase">abdullahhh33846@gmail.com</span>
            </a>
            <a href="https://github.com/abdullah-ali-338" target="_blank" class="group flex flex-col md:hairline-l md:pl-6">
                <span class="meta-label">GitHub</span>
                <span class="group-hover:underline font-bold text-sm lowercase">github.com/abdullah-ali-338</span>
            </a>
            <a href="https://www.linkedin.com/in/abdullah-ali-se" target="_blank" class="group flex flex-col md:hairline-l md:pl-6">
                <span class="meta-label">LinkedIn</span>
                <span class="group-hover:underline font-bold text-sm lowercase">linkedin.com/in/abdullah-ali-se</span>
            </a>
        </div>

        <footer class="flex flex-col md:flex-row justify-between font-mono text-[11px] text-neutral-500 uppercase tracking-widest gap-2">
            <span>Abdullah Ali</span>
            <span>2026 Developer Portfolio</span>
            <span>Object 01</span>
        </footer>
    </section>

</body>
</html>
