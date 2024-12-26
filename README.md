<style>
/* Snow Effect */
@keyframes snowfall {
    0% {
        transform: translateY(-10vh) translateX(-20px) rotate(0deg) scale(0.6);
        opacity: 0;
    }
    10% {
        opacity: 1;
        transform: translateY(0) translateX(10px) rotate(45deg) scale(0.7);
    }
    45% {
        transform: translateY(45vh) translateX(-15px) rotate(180deg) scale(0.85);
        opacity: 0.8;
    }
    80% {
        transform: translateY(80vh) translateX(15px) rotate(270deg) scale(0.9);
        opacity: 0.6;
    }
    100% {
        transform: translateY(105vh) translateX(20px) rotate(360deg) scale(1);
        opacity: 0;
    }
}

@keyframes snowflakeShine {
    0%, 100% {
        text-shadow: 
            0 0 5px rgba(255,255,255,0.8),
            0 0 10px rgba(255,255,255,0.5),
            0 0 15px rgba(255,255,255,0.3);
        filter: drop-shadow(0 0 10px rgba(255,255,255,0.5));
    }
    50% {
        text-shadow: 
            0 0 10px rgba(255,255,255,0.9),
            0 0 20px rgba(255,255,255,0.7),
            0 0 30px rgba(255,255,255,0.5),
            0 0 40px rgba(173,216,230,0.3);
        filter: drop-shadow(0 0 15px rgba(255,255,255,0.7));
    }
}

.snowflake {
    position: fixed;
    color: white;
    font-size: 1.5em;
    font-family: Arial, sans-serif;
    text-shadow: 0 0 5px rgba(255,255,255,0.8);
    user-select: none;
    z-index: 1000;
    pointer-events: none;
    will-change: transform, opacity;
    animation: 
        snowfall linear infinite,
        snowflakeShine ease-in-out infinite;
}

/* Different snowflake sizes and rotations */
.snowflake:nth-of-type(3n) { 
    font-size: 1.8em; 
    transform-origin: center center;
}
.snowflake:nth-of-type(3n+1) { 
    font-size: 1.2em;
    transform-origin: 60% 60%;
}
.snowflake:nth-of-type(3n+2) { 
    font-size: 1.5em;
    transform-origin: 40% 40%;
}

/* Enhanced snowflake positions and animations */
.snowflake:nth-child(1) { left: 5%; animation-duration: 13.5s, 4s; animation-delay: -2s, 0s; }
.snowflake:nth-child(2) { left: 15%; animation-duration: 11.8s, 3.2s; animation-delay: -4s, -1s; }
.snowflake:nth-child(3) { left: 25%; animation-duration: 14.2s, 3.5s; animation-delay: -6s, -2s; }
.snowflake:nth-child(4) { left: 35%; animation-duration: 12.4s, 4.5s; animation-delay: -1s, -3s; }
.snowflake:nth-child(5) { left: 45%; animation-duration: 15.6s, 3.2s; animation-delay: -3s, -1.5s; }
.snowflake:nth-child(6) { left: 55%; animation-duration: 13.2s, 4.2s; animation-delay: -5s, -2.5s; }
.snowflake:nth-child(7) { left: 65%; animation-duration: 14.8s, 3.8s; animation-delay: -7s, -0.5s; }
.snowflake:nth-child(8) { left: 75%; animation-duration: 12.9s, 4.8s; animation-delay: -2s, -1.8s; }
.snowflake:nth-child(9) { left: 85%; animation-duration: 15.3s, 3.4s; animation-delay: -4s, -2.2s; }
.snowflake:nth-child(10) { left: 95%; animation-duration: 13.7s, 4.4s; animation-delay: -6s, -3s; }

/* Base styles */
body {
    background: url("https://cdn.discordapp.com/attachments/1317588808799096911/1320498405562257438/Rectangle_14.png?ex=6769d179&is=67687ff9&hm=45d31d99c90f7aae717d022eb3933eca76bae509cbb1c265972726cf0883eaec&");
    color: var(--text);
    font-family: 'gg sans', 'Noto Sans', 'Helvetica Neue', Helvetica, Arial, sans-serif;
    line-height: 1.6;
    margin: 0;
    padding: 0;
}

/* Enhanced Documentation Styles */
.docs-header {
    text-align: center;
    padding: 60px 20px;
    background: rgba(0,0,0,0.3);
    border-bottom: 1px solid rgba(255,255,255,0.1);
}

.docs-header h1 {
    font-size: 4em;
    margin: 0;
    color: var(--primary);
    text-shadow: 0 0 10px rgba(250,191,55,0.3);
}

.docs-header p {
    font-size: 1.4em;
    margin: 10px 0;
    color: var(--text-secondary);
}

.badges {
    margin: 20px 0;
    display: flex;
    gap: 10px;
    justify-content: center;
}

.badge {
    padding: 5px 10px;
    border-radius: 4px;
    font-size: 0.9em;
    background: rgba(255,255,255,0.1);
    color: var(--text);
    text-decoration: none;
}

.features-section {
    padding: 40px 20px;
}

.features-list {
    display: grid;
    grid-template-columns: repeat(auto-fit, minmax(250px, 1fr));
    gap: 20px;
    margin: 20px 0;
}

.feature-item {
    background: rgba(255,255,255,0.03);
    padding: 20px;
    border-radius: 8px;
    border: 1px solid rgba(255,255,255,0.05);
    transition: transform 0.2s ease;
}

.feature-item:hover {
    transform: translateY(-2px);
    border-color: var(--primary);
}

.code-block {
    background: rgba(0,0,0,0.3);
    padding: 20px;
    border-radius: 8px;
    border: 1px solid rgba(255,255,255,0.05);
    overflow-x: auto;
    margin: 20px 0;
}

.code-block pre {
    margin: 0;
    color: #e6e6e6;
}

/* Rest of your existing styles */
</style>

<!-- Snow Effect -->
<div class="snowflake">❄</div>
<div class="snowflake">❅</div>
<div class="snowflake">❆</div>
<div class="snowflake">❄</div>
<div class="snowflake">❅</div>
<div class="snowflake">❊</div>
<div class="snowflake">❄</div>
<div class="snowflake">❅</div>
<div class="snowflake">❆</div>
<div class="snowflake">❋</div>

<!-- Documentation Header -->
<div class="docs-header">
    <h1>🌨️ Snow Theme</h1>
    <p>Add beautiful falling snowflakes to any website with a single line of code</p>
    <div class="badges">
        <span class="badge">📦 2.5kb minified</span>
        <span class="badge">⚡ Zero Dependencies</span>
        <span class="badge">🌐 Cross-Browser</span>
    </div>
</div>

<!-- Features Section -->
<div class="features-section">
    <h2>✨ Features</h2>
    <div class="features-list">
        <div class="feature-item">
            <h3>🪶 Lightweight</h3>
            <p>Only 2.5kb minified, perfect for any project</p>
        </div>
        <div class="feature-item">
            <h3>📱 Responsive</h3>
            <p>Works perfectly on all devices and screens</p>
        </div>
        <div class="feature-item">
            <h3>⚡ Zero Dependencies</h3>
            <p>Pure JavaScript, no external libraries needed</p>
        </div>
    </div>
</div>

<!-- Quick Start Section -->
<div class="container">
    <h2>🚀 Quick Start</h2>
    <div class="code-block">
        <pre><code>&lt;script src="https://ddosnotification.github.io/snow-theme/snow.js"&gt;&lt;/script&gt;</code></pre>
    </div>
    
    <!-- Rest of your existing content -->
</div>
