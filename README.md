<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0, viewport-fit=cover">
    <title>Hany Mohamed Salah · IT Support & Data Professional</title>
    <!-- Google Fonts + Font Awesome -->
    <link href="https://fonts.googleapis.com/css2?family=Inter:opsz,wght@14..32,300;14..32,400;14..32,500;14..32,600;14..32,700&display=swap" rel="stylesheet">
    <link rel="stylesheet" href="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/6.0.0-beta3/css/all.min.css">
    <style>
        * {
            margin: 0;
            padding: 0;
            box-sizing: border-box;
        }

        body {
            background: #f4f6fa;
            font-family: 'Inter', sans-serif;
            color: #1a2634;
            line-height: 1.45;
            padding: 2rem 1.5rem;
        }

        .page {
            max-width: 1280px;
            margin: 0 auto;
            background: white;
            border-radius: 2rem;
            box-shadow: 0 20px 35px -12px rgba(0,0,0,0.08);
            overflow: hidden;
            padding: 2rem 2rem 2.5rem 2rem;
            transition: all 0.2s;
        }

        /* Banner image styling */
        .banner-container {
            width: 100%;
            margin-bottom: 1.8rem;
            border-radius: 1.5rem;
            overflow: hidden;
            background: #eef2fa;
            box-shadow: 0 4px 12px rgba(0,0,0,0.03);
        }
        .banner-img {
            width: 100%;
            height: auto;
            display: block;
            object-fit: cover;
            transition: transform 0.2s ease;
        }
        .banner-img:hover {
            transform: scale(1.01);
        }

        h1 {
            font-size: 2.5rem;
            font-weight: 700;
            letter-spacing: -0.02em;
            background: linear-gradient(135deg, #1e2b3c, #0f4c5f);
            background-clip: text;
            -webkit-background-clip: text;
            color: transparent;
            margin-bottom: 0.35rem;
        }

        .subhead {
            font-size: 1.1rem;
            font-weight: 500;
            color: #2c6279;
            border-left: 4px solid #2c7da0;
            padding-left: 0.9rem;
            margin: 0.5rem 0 1rem 0;
        }

        .tagline {
            color: #4a6272;
            margin-bottom: 1.8rem;
            font-size: 1rem;
            border-bottom: 1px solid #e4e9f0;
            padding-bottom: 1rem;
        }

        .portfolio-row {
            background: #f0f4f9;
            padding: 1rem 1.4rem;
            border-radius: 60px;
            display: flex;
            flex-wrap: wrap;
            justify-content: space-between;
            align-items: center;
            gap: 0.8rem;
            margin: 1.2rem 0 2rem 0;
            font-weight: 500;
        }
        .portfolio-label {
            font-weight: 700;
            background: #1e2b3c;
            color: white;
            padding: 0.2rem 1rem;
            border-radius: 40px;
            font-size: 0.85rem;
            letter-spacing: 0.3px;
        }
        .contact-links {
            display: flex;
            flex-wrap: wrap;
            gap: 1.4rem;
            align-items: center;
            font-size: 0.95rem;
        }
        .contact-links a {
            text-decoration: none;
            color: #1e4663;
            font-weight: 500;
            transition: 0.2s;
            display: inline-flex;
            align-items: center;
            gap: 6px;
        }
        .contact-links a:hover { color: #0f6b8c; transform: translateY(-1px); }
        .location-badge {
            background: white;
            padding: 0.2rem 0.9rem;
            border-radius: 30px;
            font-size: 0.85rem;
            display: inline-flex;
            align-items: center;
            gap: 6px;
            box-shadow: 0 1px 2px rgba(0,0,0,0.05);
        }

        .pillars {
            display: grid;
            grid-template-columns: repeat(auto-fit, minmax(210px, 1fr));
            gap: 1.5rem;
            margin: 1.8rem 0 2.2rem 0;
        }
        .pillar-card {
            background: #ffffff;
            border-radius: 1.5rem;
            padding: 1.4rem 1rem;
            text-align: center;
            box-shadow: 0 6px 14px rgba(0, 0, 0, 0.02), 0 2px 4px rgba(0,0,0,0.05);
            border: 1px solid #eef2f8;
            transition: all 0.2s;
        }
        .pillar-card:hover { border-color: #cbdde9; transform: translateY(-4px); }
        .pillar-icon { font-size: 2rem; margin-bottom: 0.6rem; color: #2c7da0; }
        .pillar-card h3 { font-size: 1.25rem; font-weight: 700; margin-bottom: 0.4rem; }
        .pillar-card p { color: #4c6072; font-size: 0.85rem; }

        .two-cols {
            display: grid;
            grid-template-columns: repeat(auto-fit, minmax(280px, 1fr));
            gap: 2rem;
            margin: 2rem 0;
        }

        .section-title {
            font-size: 1.5rem;
            font-weight: 700;
            margin-bottom: 1.2rem;
            letter-spacing: -0.2px;
            display: flex;
            align-items: center;
            gap: 0.5rem;
            border-left: 4px solid #2c7da0;
            padding-left: 1rem;
        }

        .tech-badge {
            display: inline-block;
            background: #eef2fa;
            padding: 0.3rem 1rem;
            border-radius: 30px;
            font-size: 0.8rem;
            font-weight: 500;
            margin: 0.2rem 0.35rem;
            color: #1f5068;
        }

        .about-list {
            list-style: none;
            margin-top: 1rem;
        }
        .about-list li {
            margin-bottom: 0.6rem;
            padding-left: 1.5rem;
            position: relative;
        }
        .about-list li:before {
            content: "▹";
            position: absolute;
            left: 0;
            color: #2c7da0;
            font-weight: bold;
        }

        .stats-grid {
            display: flex;
            flex-wrap: wrap;
            gap: 1.8rem;
            background: #fafcff;
            border-radius: 1.5rem;
            padding: 1.2rem;
            border: 1px solid #e6edf4;
        }
        .stats-block { flex: 1; min-width: 180px; }
        .stats-block h4 { font-size: 1.1rem; margin-bottom: 1rem; font-weight: 700; border-bottom: 2px dashed #cde0ec; display: inline-block; }
        .stat-item { display: flex; justify-content: space-between; padding: 0.5rem 0; border-bottom: 1px solid #eceff5; font-size: 0.9rem; }
        .lang-progress { background: #e2e8f0; border-radius: 20px; height: 8px; width: 100%; overflow: hidden; margin: 0.3rem 0 0.6rem; }
        .lang-fill { background: #2c7da0; height: 8px; border-radius: 20px; width: 0%; }

        .projects-grid {
            display: grid;
            grid-template-columns: repeat(auto-fit, minmax(260px, 1fr));
            gap: 1.6rem;
            margin: 1.5rem 0;
        }
        .project-card {
            background: #ffffff;
            border-radius: 1.2rem;
            padding: 1.2rem;
            border: 1px solid #eef2f8;
            transition: 0.2s;
        }
        .project-card h4 { font-size: 1.2rem; margin-bottom: 0.5rem; font-weight: 700; }
        .project-card p { font-size: 0.85rem; color: #4c6072; margin: 0.5rem 0 1rem; line-height: 1.4; }
        .project-link { font-weight: 600; text-decoration: none; color: #2c7da0; display: inline-flex; align-items: center; gap: 6px; font-size: 0.85rem; }
        .project-link:hover { gap: 10px; }

        .tools-grid { display: flex; flex-wrap: wrap; gap: 0.8rem; margin-top: 0.5rem; }
        .tool-item { background: #f0f4fa; padding: 0.4rem 1rem; border-radius: 40px; font-size: 0.8rem; font-weight: 500; }

        .achievements { display: flex; flex-wrap: wrap; gap: 1.2rem; margin: 1rem 0; }
        .achievement { flex: 1; background: #f9fbfe; padding: 1rem; border-radius: 1rem; border-left: 3px solid #2c7da0; }

        .learning-item { margin-bottom: 1rem; }
        .learning-header { display: flex; justify-content: space-between; font-size: 0.85rem; font-weight: 500; margin-bottom: 0.3rem; }
        .progress-bar-bg { background: #e2e8f0; border-radius: 40px; height: 8px; width: 100%; }
        .progress-fill { background: #2c7da0; border-radius: 40px; height: 8px; width: 0%; }

        .open-role {
            background: linear-gradient(110deg, #eef5fa 0%, #ffffff 100%);
            border-radius: 2rem;
            padding: 1.2rem 1.6rem;
            text-align: center;
            border: 1px solid #d4e2ed;
            margin-top: 2rem;
            font-weight: 600;
            color: #165a72;
        }
        hr { margin: 1.5rem 0; border: 0; height: 1px; background: linear-gradient(90deg, #cbdde9, transparent); }
        @media (max-width: 700px) {
            .page { padding: 1.5rem; }
            h1 { font-size: 1.8rem; }
            .portfolio-row { flex-direction: column; align-items: flex-start; border-radius: 1.5rem; }
        }
        .icon-em { font-size: 0.9rem; margin-right: 4px; }
        a { cursor: pointer; }
        .contact-links a i { width: 1.2rem; }
    </style>
</head>
<body>
<div class="page">
    <!-- BANNER IMAGE: "Hany Mohamed Salah.png" as requested -->
    <div class="banner-container">
        <img class="banner-img" src="Hany Mohamed Salah.png" alt="Hany Mohamed Salah banner" onerror="this.style.display='none'; this.nextElementSibling?.style.setProperty('display','block');">
        <div style="display: none; text-align: center; padding: 1rem; background: #f0f4f9; border-radius: 1rem; font-size: 0.85rem; color: #2c6279;">
            <i class="fas fa-image"></i> Banner image placeholder — add "Hany Mohamed Salah.png" to your repository.
        </div>
    </div>

    <!-- Name corrected to Hany to match the banner image filename -->
    <h1>Hany Mohamed Salah</h1>
    <div class="subhead">IT SUPPORT • SYSTEM ADMINISTRATION • DATA & BI</div>
    <div class="tagline">
        Berlin-based IT professional with strong experience in IT support, system administration, troubleshooting, and data-driven reporting. 
        I combine technical problem-solving with data & BI skills to optimize operations and support smarter business decisions.
    </div>

    <!-- PORTFOLIO row (exact copy) -->
    <div class="portfolio-row">
        <span class="portfolio-label"><i class="fas fa-briefcase"></i> PORTFOLIO</span>
        <div class="contact-links">
            <span class="location-badge"><i class="fas fa-map-marker-alt"></i> Berlin, Germany</span>
            <a href="#"><i class="fas fa-envelope"></i> GMAIL</a>
            <a href="#"><i class="fas fa-phone-alt"></i> CONTACT</a>
            <a href="#"><i class="fab fa-linkedin"></i> LINKEDIN</a>
            <a href="#"><i class="fas fa-share-alt"></i> CONNECT</a>
        </div>
    </div>

    <!-- Four core pillars -->
    <div class="pillars">
        <div class="pillar-card"><div class="pillar-icon"><i class="fas fa-microchip"></i></div><h3>Problem Solver</h3><p>Troubleshoot, analyze & fix</p></div>
        <div class="pillar-card"><div class="pillar-icon"><i class="fas fa-chart-line"></i></div><h3>Data Driven</h3><p>Turn data into decisions</p></div>
        <div class="pillar-card"><div class="pillar-icon"><i class="fas fa-cogs"></i></div><h3>Process Optimizer</h3><p>Improve efficiency & workflows</p></div>
        <div class="pillar-card"><div class="pillar-icon"><i class="fas fa-users"></i></div><h3>Team Player</h3><p>Collaborate & deliver value</p></div>
    </div>

    <!-- TECH STACK -->
    <div>
        <div class="section-title"><i class="fas fa-code"></i> TECH STACK</div>
        <div>
            <span class="tech-badge">Windows</span>
            <span class="tech-badge">Microsoft 365</span>
            <span class="tech-badge">Active Directory</span>
            <span class="tech-badge">Power BI</span>
            <span class="tech-badge">Python</span>
            <span class="tech-badge">Excel</span>
            <span class="tech-badge">SQL / MySQL</span>
            <span class="tech-badge">Networking</span>
            <span class="tech-badge">Git & GitHub</span>
            <span class="tech-badge">Jira</span>
        </div>
    </div>

    <!-- Two columns: About Me + GitHub Stats -->
    <div class="two-cols">
        <div>
            <div class="section-title"><i class="fas fa-user-astronaut"></i> ABOUT ME</div>
            <p style="margin-bottom: 1rem;">I help organizations run smoother IT operations and make better decisions with data. My background combines hands-on IT support & system administration with data analytics and BI reporting.</p>
            <ul class="about-list">
                <li>IT Support & Troubleshooting</li>
                <li>System Administration & Microsoft 365</li>
                <li>Active Directory • Networking Basics</li>
                <li>Data Analysis with Python & SQL</li>
                <li>Power BI Dashboards & Reporting</li>
                <li>Documentation & Process Optimization</li>
            </ul>
        </div>
        <div>
            <div class="section-title"><i class="fab fa-github"></i> GITHUB STATS</div>
            <div class="stats-grid">
                <div class="stats-block">
                    <h4>📊 Overall Stats</h4>
                    <div class="stat-item"><span>Total Repos</span><span><strong>21</strong></span></div>
                    <div class="stat-item"><span>Total Commits</span><span><strong>361</strong></span></div>
                    <div class="stat-item"><span>Total PRs</span><span><strong>18</strong></span></div>
                    <div class="stat-item"><span>Issues Closed</span><span><strong>26</strong></span></div>
                    <div class="stat-item"><span>Contributions (This Year)</span><span><strong>248+</strong> <span style="font-size:0.7rem;">active</span></span></div>
                </div>
                <div class="stats-block">
                    <h4>🏆 Top Languages</h4>
                    <div><span>Python 49.7%</span><div class="lang-progress"><div class="lang-fill" style="width:49.7%"></div></div></div>
                    <div><span>SQL 16.9%</span><div class="lang-progress"><div class="lang-fill" style="width:16.9%"></div></div></div>
                    <div><span>PowerShell 12.2%</span><div class="lang-progress"><div class="lang-fill" style="width:12.2%"></div></div></div>
                    <div><span>Other 21.2%</span><div class="lang-progress"><div class="lang-fill" style="width:21.2%"></div></div></div>
                </div>
            </div>
        </div>
    </div>

    <!-- FEATURED PROJECTS -->
    <div>
        <div class="section-title"><i class="fas fa-laptop-code"></i> FEATURED PROJECTS</div>
        <div class="projects-grid">
            <div class="project-card"><h4>📊 Business Operations Dashboard</h4><p>Power BI dashboard for tracking rent, revenue, utilization, planning and KPI performance.</p><a href="#" class="project-link">View Project →</a></div>
            <div class="project-card"><h4>📈 Demand Forecasting Analysis</h4><p>Python driven forecasting and analysis for automotive parts demand and supply chain planning.</p><a href="#" class="project-link">View Project →</a></div>
            <div class="project-card"><h4>🎯 Sales & Performance Dashboard</h4><p>Interactive Power BI dashboard for sales performance, targets, regions and product analytics.</p><a href="#" class="project-link">View Project →</a></div>
            <div class="project-card"><h4>🛠️ IT Support Toolkit</h4><p>Collection of IT troubleshooting guides, scripts, checklists and best practices for daily support tasks.</p><a href="#" class="project-link">View Project →</a></div>
        </div>
    </div>

    <!-- TOOLS & ENVIRONMENTS + ACHIEVEMENTS -->
    <div class="two-cols" style="margin-top: 0.5rem;">
        <div>
            <div class="section-title"><i class="fas fa-tools"></i> TOOLS & ENVIRONMENTS</div>
            <div class="tools-grid">
                <span class="tool-item">Windows 10/11</span>
                <span class="tool-item">Microsoft 365 (Outlook, Teams)</span>
                <span class="tool-item">Remote Support AnyDesk, RDP</span>
                <span class="tool-item">Virtualization VMware, Hyper-V</span>
                <span class="tool-item">Active Directory DNS, DHCP</span>
                <span class="tool-item">Network TCP/IP, VPN</span>
            </div>
        </div>
        <div>
            <div class="section-title"><i class="fas fa-medal"></i> ACHIEVEMENTS</div>
            <div class="achievements">
                <div class="achievement"><strong>🌟 Consistent Contributor</strong><p style="font-size:0.8rem; margin-top:4px;">Maintaining an active contribution streak</p></div>
                <div class="achievement"><strong>⚡ Problem Solver</strong><p style="font-size:0.8rem; margin-top:4px;">Resolved numerous IT issues & incidents</p></div>
                <div class="achievement"><strong>📊 Data Enthusiast</strong><p style="font-size:0.8rem; margin-top:4px;">Turning data into insights & reports</p></div>
            </div>
        </div>
    </div>

    <!-- CURRENTLY LEARNING (percentages) -->
    <div style="margin: 1rem 0 0.8rem 0;">
        <div class="section-title"><i class="fas fa-graduation-cap"></i> CURRENTLY LEARNING</div>
        <div style="display: grid; gap: 1rem; grid-template-columns: repeat(auto-fit, minmax(220px,1fr));">
            <div class="learning-item"><div class="learning-header"><span>Advanced Power BI & DAX</span><span>70%</span></div><div class="progress-bar-bg"><div class="progress-fill" style="width:70%"></div></div></div>
            <div class="learning-item"><div class="learning-header"><span>Azure Fundamentals</span><span>60%</span></div><div class="progress-bar-bg"><div class="progress-fill" style="width:60%"></div></div></div>
            <div class="learning-item"><div class="learning-header"><span>Python for Data Engineering</span><span>65%</span></div><div class="progress-bar-bg"><div class="progress-fill" style="width:65%"></div></div></div>
            <div class="learning-item"><div class="learning-header"><span>Linux & Server Administration</span><span>50%</span></div><div class="progress-bar-bg"><div class="progress-fill" style="width:50%"></div></div></div>
        </div>
    </div>

    <!-- Open for roles callout -->
    <div class="open-role">
        <i class="fas fa-map-pin"></i> Open to IT Support, System Administration, Data & BI roles in Berlin and Remote.
    </div>

    <hr />
    <div style="font-size: 0.7rem; text-align: center; color: #8ba0ae; margin-top: 0.8rem;">
        <i class="fas fa-code-branch"></i> portfolio • Berlin-based • always building
    </div>
</div>
</body>
</html>
