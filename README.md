<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Lance Gabriel Reyes | Computer Engineering</title>
    <style>
        :root {
            --bg-primary: #0a0e17;
            --bg-secondary: #131a26;
            --accent-cyan: #00f2fe;
            --accent-green: #4af626;
            --text-main: #c9d1d9;
            --text-muted: #8b949e;
            --border-color: #21262d;
        }

        * { box-sizing: border-box; margin: 0; padding: 0; }
        body { 
            font-family: 'Courier New', Courier, monospace; 
            background-color: var(--bg-primary); 
            color: var(--text-main); 
            line-height: 1.6; 
            padding: 20px;
        }

        .terminal-window {
            max-width: 900px;
            margin: 40px auto;
            background-color: var(--bg-secondary);
            border: 1px solid var(--border-color);
            border-radius: 6px;
            box-shadow: 0 10px 30px rgba(0,0,0,0.5);
            overflow: hidden;
        }

        .terminal-header {
            background-color: #161b22;
            padding: 10px 15px;
            border-bottom: 1px solid var(--border-color);
            display: flex;
            align-items: center;
        }

        .terminal-buttons {
            display: flex;
            gap: 8px;
            margin-right: 15px;
        }

        .dot { width: 12px; height: 12px; border-radius: 50%; }
        .dot-red { background-color: #ff5f56; }
        .dot-yellow { background-color: #ffbd2e; }
        .dot-green { background-color: #27c93f; }
        .terminal-title { font-size: 0.85rem; color: var(--text-muted); }

        .terminal-body { padding: 30px; }

        /* System Info Banner */
        .sys-info { margin-bottom: 30px; color: var(--text-muted); font-size: 0.9rem; }
        .sys-info span { color: var(--accent-cyan); }

        /* Commands */
        .command-prompt { color: var(--accent-green); margin-top: 25px; margin-bottom: 10px; font-weight: bold; }
        .command-prompt::before { content: "lance@cpe-desktop:~$ "; color: var(--accent-cyan); }

        h1 { font-size: 2rem; color: #fff; margin-bottom: 5px; }
        .highlight { color: var(--accent-cyan); }
        
        /* Grid Sections */
        .grid-2 { display: grid; grid-template-columns: repeat(auto-fit, minmax(300px, 1fr)); gap: 20px; }
        
        .card {
            background-color: var(--bg-primary);
            border: 1px solid var(--border-color);
            padding: 20px;
            border-radius: 4px;
            position: relative;
        }
        .card:hover { border-color: var(--accent-cyan); }
        .card-title { color: #fff; font-size: 1.1rem; margin-bottom: 10px; font-weight: bold; }
        
        .tech-badge {
            display: inline-block;
            font-size: 0.75rem;
            background: #21262d;
            color: var(--accent-cyan);
            padding: 2px 8px;
            border-radius: 3px;
            margin-right: 5px;
            margin-top: 5px;
        }

        a { color: var(--accent-green); text-decoration: none; font-size: 0.9rem; }
        a:hover { text-decoration: underline; }
        
        ul { list-style-type: none; }
        ul li::before { content: "⚡ "; color: var(--accent-cyan); }

        footer { text-align: center; margin-top: 40px; color: var(--text-muted); font-size: 0.8rem; }
    </style>
</head>
<body>

    <div class="terminal-window">
        <!-- Window Controls Window Chrome Header -->
        <div class="terminal-header">
            <div class="terminal-buttons">
                <div class="dot dot-red"></div>
                <div class="dot dot-yellow"></div>
                <div class="dot dot-green"></div>
            </div>
            <div class="terminal-title">bash — lance@cpe-desktop:~/portfolio</div>
        </div>

        <div class="terminal-body">
            <!-- System Printout Info -->
            <div class="sys-info">
                Last login: Monday June 2026 on ttys001<br>
                [System Profile]: <span class="highlight">Lance Gabriel Reyes</span><br>
                [Department]: <span>Computer Engineering (CpE) - 2nd Year Undergraduate</span><br>
                [Timeline]: <span>Expected Graduation Node: June 2028</span>
            </div>

            <h1>LANCE_GABRIEL_REYES.init()</h1>
            <p style="color: var(--text-muted);">Focusing on low-level system designs, digital logic layouts, and deep-end structural hardware-software engineering integration blueprints.</p>

            <!-- Skills Section -->
            <div class="command-prompt">cat skills.json</div>
            <div class="card">
                <div style="margin-bottom: 10px;"><strong class="highlight">[Languages]:</strong> Python, C, C++, ARM Assembly, HTML/CSS</div>
                <div style="margin-bottom: 10px;"><strong class="highlight">[Hardware/Tools]:</strong> Verilog HDL, Git, Linux Environment, Microcontrollers (ESP32/Arduino)</div>
                <div><strong class="highlight">[Frameworks]:</strong> Django REST Framework, SQLite</div>
            </div>

            <!-- Current Academic Tracks -->
            <div class="command-prompt">ls -la core_courses/</div>
            <div class="grid-2">
                <div class="card">
                    <div class="card-title">Completed Blocks</div>
                    <ul>
                        <li>Object-Oriented Coding</li>
                        <li>Discrete Mathematics</li>
                        <li>Data Structures & Algos</li>
                    </ul>
                </div>
                <div class="card">
                    <div class="card-title">In-Flight Track (Year 2)</div>
                    <ul>
                        <li>Digital Design & Logic Systems</li>
                        <li>Microprocessor Architectures</li>
                        <li>Electronic Circuit Elements</li>
                    </ul>
                </div>
            </div>

            <!-- Projects Section -->
            <div class="command-prompt">git log --oneline --project-space</div>
            <div class="grid-2">
                <!-- Project Node 1 -->
                <div class="card">
                    <div class="card-title">0x01: RTOS Task Scheduler Core</div>
                    <p style="font-size:0.85rem; color: var(--text-muted); margin-bottom:15px;">Simulated dynamic context switches and thread prioritizing calculations built natively via Python processing modules.</p>
                    <div>
                        <span class="tech-badge">Python</span>
                        <span class="tech-badge">OS Concepts</span>
                    </div>
                    <div style="margin-top:15px;"><a href="https://github.com/LanceGabrielReyes" target="_blank">[View Source]</a></div>
                </div>

                <!-- Project Node 2 -->
                <div class="card">
                    <div class="card-title">0x02: Custom Django Hardware Logger</div>
                    <p style="font-size:0.85rem; color: var(--text-muted); margin-bottom:15px;">Asynchronous pipeline recording simulated peripheral system metrics directly using lightweight relational backends.</p>
                    <div>
                        <span class="tech-badge">Django</span>
                        <span class="tech-badge">SQLite</span>
                    </div>
                    <div style="margin-top:15px;"><a href="https://github.com/LanceGabrielReyes" target="_blank">[View Source]</a></div>
                </div>
            </div>

            <div class="command-prompt"><span class="dot-green" style="display:inline-block; width:10px; height:10px; border-radius:50%; animation: blink 1s infinite;"></span></div>
        </div>
    </div>

    <footer>
        <p>Executed safely using system elements. © 2026 Lance Gabriel Reyes</p>
    </footer>

    <script>
        // Blinking terminal prompt cursor effect
        setInterval(() => {
            const cursor = document.querySelector('.command-prompt .dot-green');
            if(cursor) cursor.style.opacity = cursor.style.opacity === '0' ? '1' : '0';
        }, 600);
    </script>
</body>
</html>
