<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Document</title>
    <style>
        /* --- GITHUB README PROFILE (NEO STYLE) --- */
        .github-profile-container {
            background: rgba(18, 18, 18, 0.6); /* Dark glass */
            border: 1px solid var(--glass-border);
            border-top: 2px solid var(--neon-purple); /* Top border highlight */
            border-radius: 10px;
            padding: 40px;
            position: relative;
            overflow: hidden;
            box-shadow: 0 0 20px rgba(0, 0, 0, 0.5);
            font-family: 'Space Mono', monospace; /* Code font */
        }

        /* Scanline Effect Overlay */
        .github-profile-container::before {
            content: " ";
            display: block;
            position: absolute;
            top: 0; left: 0; bottom: 0; right: 0;
            background: linear-gradient(rgba(18, 16, 16, 0) 50%, rgba(0, 0, 0, 0.25) 50%), linear-gradient(90deg, rgba(255, 0, 0, 0.06), rgba(0, 255, 0, 0.02), rgba(0, 0, 255, 0.06));
            z-index: 2;
            background-size: 100% 2px, 3px 100%;
            pointer-events: none;
        }

        /* Typing SVG Wrapper */
        .typing-header {
            text-align: center;
            margin-bottom: 40px;
            position: relative;
            z-index: 3;
        }

        /* Section Headers */
        .neo-h3 {
            color: var(--neon-cyan);
            font-size: 1.5rem;
            margin-bottom: 1rem;
            display: flex;
            align-items: center;
            gap: 10px;
            border-bottom: 1px dashed rgba(0, 243, 255, 0.3);
            padding-bottom: 10px;
        }

        /* Neo Skills Table */
        .skills-matrix {
            width: 100%;
            border-collapse: separate;
            border-spacing: 0 15px; /* Space between rows */
            margin-bottom: 40px;
            position: relative;
            z-index: 3;
        }

        .skills-matrix td {
            background: rgba(0, 0, 0, 0.3);
            border: 1px solid var(--glass-border);
            padding: 20px;
            vertical-align: top;
            width: 50%;
            border-radius: 5px;
            transition: 0.3s;
        }

        .skills-matrix td:hover {
            border-color: var(--neon-purple);
            box-shadow: 0 0 15px rgba(188, 19, 254, 0.2);
            transform: translateY(-2px);
        }

        .skills-category {
            color: var(--neon-pink);
            font-size: 1.1rem;
            margin-bottom: 10px;
            display: block;
            font-weight: bold;
        }

        .skill-list li {
            color: var(--text-muted);
            margin-bottom: 5px;
            list-style-type: none;
            padding-left: 20px;
            position: relative;
        }
        .skill-list li::before {
            content: '>';
            color: var(--neon-cyan);
            position: absolute;
            left: 0;
            font-weight: bold;
        }

        /* Tech Tags / Chips */
        .tech-tag-container {
            display: flex; flex-wrap: wrap; gap: 10px; margin-bottom: 40px; position: relative; z-index: 3;
        }
        .tech-tag {
            background: rgba(255, 255, 255, 0.05);
            border: 1px solid var(--neon-cyan);
            color: var(--neon-cyan);
            padding: 5px 15px;
            border-radius: 20px;
            font-size: 0.9rem;
            transition: 0.3s;
            cursor: default;
        }
        .tech-tag:hover {
            background: var(--neon-cyan);
            color: #000;
            box-shadow: 0 0 10px var(--neon-cyan);
        }

        /* Career Objective Terminal */
        .career-terminal {
            background: #000;
            border-left: 4px solid var(--neon-purple);
            padding: 20px;
            margin-top: 20px;
            font-family: 'Space Mono', monospace;
            color: var(--text-main);
            position: relative;
            z-index: 3;
        }
        .career-terminal::before {
            content: '$ ./run_objective.exe';
            display: block;
            color: var(--text-muted);
            margin-bottom: 10px;
            font-size: 0.8rem;
        }
    </style>
</head>
<body>
    <!-- GitHub README / Neo Profile Section -->
    <section id="github-profile" class="block">
        <div class="container">
            <div class="github-profile-container">
                
                <!-- Typing SVG Header -->
                <div class="typing-header reveal">
                    <p align="center"> 
                        <img src="https://readme-typing-svg.demolab.com?font=Segoe+UI&size=28&duration=3000&pause=1000&color=0E75B6&center=true&vCenter=true&width=800&lines=Undergraduate+IT+Student;Aspiring+Software+Engineer;Database+%26+Networking+Enthusiast;Always+Learning+New+Technologies" alt="Typing SVG" /> 
                    </p>
                </div>

                <!-- About Me -->
                <div class="reveal delay-100">
                    <h3 class="neo-h3">👨‍🎓 About Me</h3>
                    <div class="text-secondary" style="line-height: 1.8;">
                        <p>🎓 Undergraduate Student passionate about Information Technology</p>
                        <p>💻 Interested in Software Development, Databases & Networking</p>
                        <p>🚀 Focused on building practical, real-world technical skills</p>
                        <p style="margin-top:15px; border-left: 2px solid var(--neon-pink); padding-left: 15px;">
                            I continuously work on improving my knowledge in backend development, database systems, and network architecture.
                        </p>
                    </div>
                </div>

                <!-- Technical Skills Matrix -->
                <div class="reveal delay-200">
                    <h3 class="neo-h3">🛠️ Technical Skills</h3>
                    
                    <table class="skills-matrix">
                        <tr>
                            <td>
                                <span class="skills-category">💻 Programming</span>
                                <ul class="skill-list">
                                    <li>C#</li>
                                    <li>SQL (MS SQL Server, SQLite)</li>
                                    <li>Python</li>
                                    <li>HTML & CSS</li>
                                </ul>
                            </td>
                            <td>
                                <span class="skills-category">🗄️ Database</span>
                                <ul class="skill-list">
                                    <li>Database Normalization</li>
                                    <li>ER Modeling</li>
                                    <li>Constraints & Relationships</li>
                                    <li>Query Optimization</li>
                                </ul>
                            </td>
                        </tr>
                        <tr>
                            <td>
                                <span class="skills-category">🌐 Networking</span>
                                <ul class="skill-list">
                                    <li>TCP/IP Model</li>
                                    <li>DNS, DHCP, HTTP</li>
                                    <li>Cisco Packet Tracer</li>
                                    <li>Wireless Networking</li>
                                </ul>
                            </td>
                            <td>
                                <span class="skills-category">🖥️ Tools</span>
                                <ul class="skill-list">
                                    <li>Git & GitHub</li>
                                    <li>Visual Studio</li>
                                    <li>Visual Studio Code</li>
                                    <li>SQL Server Management Studio (SSMS)</li>
                                    <li>MySQL Server</li>
                                    <li>Kali Linux</li>
                                    <li>Microsoft Visio</li>
                                </ul>
                            </td>
                        </tr>
                    </table>
                </div>

                <!-- Projects & Learning -->
                <div class="reveal delay-300">
                    <h3 class="neo-h3">📂 Projects & Learning</h3>
                    
                    <p style="color:var(--neon-purple); margin-bottom:10px;">Academic & Personal Projects:</p>
                    <div class="tech-tag-container">
                        <div class="tech-tag">🔹 Student Management System (DB Design)</div>
                        <div class="tech-tag">🔹 Network Topology Design</div>
                        <div class="tech-tag">🔹 Arduino Bluetooth Car</div>
                    </div>

                    <p style="color:var(--neon-purple); margin-bottom:10px;">Currently Learning:</p>
                    <div class="tech-tag-container">
                        <div class="tech-tag">Advanced SQL (Procedures)</div>
                        <div class="tech-tag">Authentication Systems</div>
                        <div class="tech-tag">GitHub Workflow</div>
                        <div class="tech-tag">Secure Architecture</div>
                    </div>
                </div>

                <!-- Career Objective -->
                <div class="reveal delay-400">
                    <h3 class="neo-h3">🎯 Career Objective</h3>
                    <div class="career-terminal">
                        <p>To grow into a highly skilled Software Engineer / System Engineer capable of designing secure, scalable, and efficient systems.</p>
                        <br>
                        <p>⭐ Committed to continuous improvement and professional growth.</p>
                    </div>
                </div>

            </div>
        </div>
    </section>
</body>
</html>
