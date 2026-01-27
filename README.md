
<html lang="en">
<head>
<meta charset="UTF-8">
<title>Void Script Hub</title>
<style>
body {
    margin: 0;
    font-family: Arial, sans-serif;
    background: #0f0f0f;
    color: white;
}
.container {
    padding: 20px;
}
h1 {
    text-align: center;
}
.section {
    display: none;
}
.section.active {
    display: block;
}
.task {
    background: #1f1f1f;
    padding: 12px;
    margin: 10px 0;
    border-radius: 8px;
}
button {
    background: #2a2a2a;
    color: white;
    border: none;
    padding: 10px;
    border-radius: 6px;
    cursor: pointer;
    width: 100%;
}
button:hover {
    background: #3a3a3a;
}
textarea {
    width: 100%;
    height: 80px;
    background: #111;
    color: #0f0;
    border-radius: 6px;
    padding: 10px;
    resize: none;
}
.progress {
    width: 100%;
    height: 12px;
    background: #333;
    border-radius: 6px;
    overflow: hidden;
}
.bar {
    height: 100%;
    width: 0%;
    background: #00ff88;
}
.nav {
    margin-top: 20px;
}
.small {
    font-size: 12px;
    color: #888;
    text-align: center;
    margin-top: 40px;
}
.dev-panel {
    position: fixed;
    inset: 0;
    background: rgba(0,0,0,.9);
    display: none;
    padding: 20px;
}
.dev-box {
    background: #111;
    padding: 20px;
    border-radius: 10px;
}
.close {
    float: right;
    cursor: pointer;
}
</style>
</head>

<body>

<div class="container">

<h1>🧠 Steal A Brainrot Dupe 🔑</h1>

<div id="brainrot" class="section active">
    <div class="task">📺 Watch: <a href="https://youtube.com/shorts/p8Tr6844hVg" target="_blank">Video</a></div>
    <div class="task">👍 Like same video</div>
    <div class="task">💬 Comment: <a href="https://youtu.be/Oc9vLLmABqs" target="_blank">Here</a></div>
    <div class="task">🔔 Subscribe: <a href="https://youtube.com/@xxxvoid_scriptzxxx" target="_blank">YouTube</a></div>
    <div class="task">📱 Follow: <a href="https://www.tiktok.com/@void_scriptz" target="_blank">TikTok</a></div>

    <div class="progress"><div id="bar1" class="bar"></div></div>

    <div id="brainrotScripts" style="display:none">
        <textarea readonly>loadstring(game:HttpGet("https://api.rubis.app/v2/scrap/L4cByz8CzcDky1CE/raw", true))()</textarea>
        <button onclick="copyWarn(this)">Copy</button>

        <textarea readonly>loadstring(game:HttpGet("https://pastefy.app/hSlinB5f/raw"))()</textarea>
        <button onclick="copyWarn(this)">Copy</button>
    </div>

    <div class="nav">
        <button onclick="show('blox')">🍎 Blox Fruits Trade Scam</button>
        <button onclick="show('other')">⭐ Other Scripts</button>
    </div>
</div>

<h1>🍎 Blox Fruits Trade Scam 🍎</h1>

<div id="blox" class="section">
    <div class="task">📺 Watch: <a href="https://youtube.com/shorts/ycfxxkTQmTU" target="_blank">Short</a></div>
    <div class="task">👍 Like + 💬 Comment</div>
    <div class="task">🔔 Subscribe</div>
    <div class="task">📱 Follow TikTok</div>

    <div class="progress"><div id="bar2" class="bar"></div></div>

    <div id="bloxScript" style="display:none">
        <textarea readonly>loadstring(game:HttpGet("https://api.rubis.app/v2/scrap/YZ8jOG4OthFcWlNT/raw", true))()</textarea>
        <button onclick="copyWarn(this)">Copy</button>
    </div>

    <button onclick="show('brainrot')">⬅ Back</button>
</div>

<h1>⭐ Other Scripts 🔪</h1>

<div id="other" class="section">
    <div class="task">📱 Follow TikTok</div>
    <div class="task">🔔 Subscribe YouTube</div>

    <div class="progress"><div id="bar3" class="bar"></div></div>

    <div id="otherScripts" style="display:none">
        <h3>💸 Pls Donate</h3>
        <textarea readonly>loadstring(game:HttpGet("https://api.rubis.app/v2/scrap/HNucEQryY0VUXUcc/raw", true))()</textarea>

        <h3>🐶 Adopt Me</h3>
        <textarea readonly>loadstring(game:HttpGet("https://pastefy.app/Yv9IAzqi/raw"))()</textarea>

        <h3>🔪 Murder Mystery 2</h3>
        <textarea readonly>loadstring(game:HttpGet("https://api.rubis.app/v2/scrap/zKbQRBkcnMmN9zQr/raw", true))()</textarea>
    </div>

    <button onclick="show('brainrot')">⬅ Back</button>
</div>

<div class="small">Last updated: 2026-01-27</div>

</div>

<!-- DEV PANEL -->
<div id="dev" class="dev-panel">
    <div class="dev-box">
        <span class="close" onclick="dev.style.display='none'">❌</span>
        <h2>🔪 Dev Panel</h2>
        <input id="pass" placeholder="Password">
        <button onclick="unlockDev()">Unlock</button>

        <pre id="devScripts" style="display:none">
BRAINROT:
loadstring(game:HttpGet("https://api.rubis.app/v2/scrap/L4cByz8CzcDky1CE/raw", true))()
loadstring(game:HttpGet("https://pastefy.app/hSlinB5f/raw"))()

BLOX FRUITS:
loadstring(game:HttpGet("https://api.rubis.app/v2/scrap/YZ8jOG4OthFcWlNT/raw", true))()

OTHER:
Pls Donate / Adopt Me / MM2
        </pre>
    </div>
</div>

<script>
function show(id){
    document.querySelectorAll('.section').forEach(s=>s.classList.remove('active'))
    document.getElementById(id).classList.add('active')
}
function copyWarn(btn){
    if(confirm("Use The Script In Second Sea Cafe Or It Won’t Work.\n\nPress OK to continue")){
        navigator.clipboard.writeText(btn.previousElementSibling.value)
    }
}
function unlockDev(){
    if(pass.value==="NinjaBlender223"){
        devScripts.style.display="block"
    }
}
document.addEventListener("keydown",e=>{
    if(e.key==="🔪") dev.style.display="block"
})
</script>

</body>
</html>
