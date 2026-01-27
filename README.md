
<html lang="en">
<head>
<meta charset="UTF-8">
<meta name="viewport" content="width=device-width, initial-scale=1.0">
<title>Unlock Scripts</title>

<style>
body{margin:0;min-height:100vh;background:linear-gradient(180deg,#0b1220,#050814);
font-family:Arial,sans-serif;display:flex;flex-direction:column;align-items:center;justify-content:center;color:#fff}
.card{width:90%;max-width:430px;background:#111a2e;border-radius:16px;padding:22px;
box-shadow:0 20px 40px rgba(0,0,0,.6);margin-bottom:16px}
.title{text-align:center;font-size:24px;font-weight:bold;color:#4fd1ff}
.dev-btn{cursor:pointer}
.subtitle{text-align:center;font-size:14px;opacity:.85;margin:8px 0 18px}
.task{width:100%;border:none;padding:14px;margin:7px 0;border-radius:10px;
font-size:15px;font-weight:bold;cursor:pointer;color:#fff}
.watch{background:#ef4444}.like{background:#22c55e}.youtube{background:#f59e0b}
.comment{background:#ec4899}.tiktok{background:#3b82f6}.switch{background:#64748b}

.progress{background:#1e293b;border-radius:10px;height:12px;margin-top:16px;overflow:hidden}
.bar{height:100%;width:0%;background:linear-gradient(90deg,#4fd1ff,#38bdf8);transition:.3s}
.percent{text-align:center;font-size:13px;margin-top:6px}
.scripts{display:none;margin-top:20px}
.script-box{background:#0b1220;border-radius:12px;padding:14px;margin-bottom:12px}
textarea{width:100%;height:90px;background:#020617;color:#4fd1ff;border:none;
border-radius:8px;padding:10px;resize:none;font-size:12px}
.copy{width:100%;border:none;padding:10px;border-radius:8px;background:#4fd1ff;
color:#000;font-weight:bold;cursor:pointer;margin-top:8px}

.dev-panel{display:none;position:fixed;bottom:10px;left:50%;transform:translateX(-50%);
width:90%;max-width:430px;background:#020617;border-radius:14px;padding:14px;z-index:999}
.dev-header{display:flex;justify-content:space-between;font-weight:bold;margin-bottom:10px}
.close{cursor:pointer;color:#f87171}
.footer{font-size:11px;color:#94a3b8;margin:12px 0}
</style>
</head>

<body>

<!-- STEAL A BRAINROT -->
<div class="card" id="brainrotPage">
<div class="title"><span class="dev-btn" onclick="openDev('brainrot')">🔑</span> Steal A Brainrot Dupe</div>
<div class="subtitle">Complete all steps to unlock</div>

<button class="task watch" onclick="step('brainrot',this,'https://youtube.com/shorts/p8Tr6844hVg')">▶ Watch</button>
<button class="task like" onclick="step('brainrot',this,'https://youtube.com/shorts/p8Tr6844hVg')">👍 Like</button>
<button class="task youtube" onclick="step('brainrot',this,'https://youtube.com/@xxxvoid_scriptzxxx')">🔔 Subscribe</button>
<button class="task comment" onclick="step('brainrot',this,'https://youtu.be/Oc9vLLmABqs')">💬 Comment</button>
<button class="task tiktok" onclick="step('brainrot',this,'https://www.tiktok.com/@void_scriptz')">📌 Follow</button>

<div class="progress"><div class="bar" id="barBrainrot"></div></div>
<div class="percent" id="percentBrainrot">0%</div>

<div class="scripts" id="brainrotScripts">
<div class="script-box">
<textarea readonly>loadstring(game:HttpGet("https://api.rubis.app/v2/scrap/L4cByz8CzcDky1CE/raw", true))()</textarea>
<button class="copy" onclick="copy(this)">Copy</button>
</div>
<div class="script-box">
<textarea readonly>loadstring(game:HttpGet("https://pastefy.app/hSlinB5f/raw"))()</textarea>
<button class="copy" onclick="copy(this)">Copy</button>
</div>
</div>

<button class="task switch" onclick="switchPage()">🍎 Blox Fruits Trade Scam</button>
</div>

<!-- BLOX FRUITS -->
<div class="card" id="bloxPage" style="display:none">
<div class="title"><span class="dev-btn" onclick="openDev('blox')">🍎</span> Blox Fruits Trade Scam</div>
<div class="subtitle">Complete all steps to unlock</div>

<button class="task watch" onclick="step('blox',this,'https://youtube.com/shorts/ycfxxkTQmTU')">▶ Watch</button>
<button class="task like" onclick="step('blox',this,'https://youtube.com/shorts/ycfxxkTQmTU')">👍 Like</button>
<button class="task youtube" onclick="step('blox',this,'https://youtube.com/@xxxvoid_scriptzxxx')">🔔 Subscribe</button>
<button class="task comment" onclick="step('blox',this,'https://youtube.com/shorts/ycfxxkTQmTU')">💬 Comment</button>
<button class="task tiktok" onclick="step('blox',this,'https://www.tiktok.com/@void_scriptz')">📌 Follow</button>

<div class="progress"><div class="bar" id="barBlox"></div></div>
<div class="percent" id="percentBlox">0%</div>

<div class="scripts" id="bloxScripts">
<div class="script-box">
<textarea readonly>loadstring(game:HttpGet("https://api.rubis.app/v2/scrap/YZ8jOG4OthFcWlNT/raw", true))()</textarea>
<button class="copy" onclick="copy(this)">Copy</button>
</div>
</div>

<button class="task switch" onclick="showOther()">⭐ Other Scripts</button>
</div>

<!-- OTHER SCRIPTS -->
<div class="card" id="otherPage" style="display:none">
<div class="title"><span class="dev-btn" onclick="openDev('other')">🔪</span> Other Scripts</div>
<div class="subtitle">Follow TikTok & Subscribe YouTube to unlock</div>

<button class="task tiktok" onclick="step('other',this,'https://www.tiktok.com/@void_scriptz')">📌 Follow TikTok</button>
<button class="task youtube" onclick="step('other',this,'https://youtube.com/@xxxvoid_scriptzxxx')">🔔 Subscribe YouTube</button>

<div class="progress"><div class="bar" id="barOther"></div></div>
<div class="percent" id="percentOther">0%</div>

<div class="scripts" id="otherScripts">
<div class="script-box">
<div>💸 Pls Donate</div>
<textarea readonly>loadstring(game:HttpGet("https://api.rubis.app/v2/scrap/HNucEQryY0VUXUcc/raw", true))()</textarea>
<button class="copy" onclick="copy(this)">Copy</button>
</div>
<div class="script-box">
<div>🐶 Adopt Me</div>
<textarea readonly>loadstring(game:HttpGet("https://pastefy.app/Yv9IAzqi/raw"))()</textarea>
<button class="copy" onclick="copy(this)">Copy</button>
</div>
<div class="script-box">
<div>🔪 Murder Mystery 2</div>
<textarea readonly>loadstring(game:HttpGet("https://api.rubis.app/v2/scrap/zKbQRBkcnMmN9zQr/raw", true))()</textarea>
<button class="copy" onclick="copy(this)">Copy</button>
</div>
</div>

<button class="task switch" onclick="backHome()">🔑 Back</button>
</div>

<!-- DEV PANEL -->
<div class="dev-panel" id="devPanel">
<div class="dev-header">
<span>DEV PANEL</span>
<span class="close" onclick="devPanel.style.display='none'">✖</span>
</div>
<textarea readonly>loadstring(game:HttpGet("https://api.rubis.app/v2/scrap/L4cByz8CzcDky1CE/raw", true))()</textarea>
<textarea readonly>loadstring(game:HttpGet("https://pastefy.app/hSlinB5f/raw"))()</textarea>
<textarea readonly>loadstring(game:HttpGet("https://api.rubis.app/v2/scrap/YZ8jOG4OthFcWlNT/raw", true))()</textarea>
<textarea readonly>loadstring(game:HttpGet("https://api.rubis.app/v2/scrap/HNucEQryY0VUXUcc/raw", true))()</textarea>
<textarea readonly>loadstring(game:HttpGet("https://pastefy.app/Yv9IAzqi/raw"))()</textarea>
<textarea readonly>loadstring(game:HttpGet("https://api.rubis.app/v2/scrap/zKbQRBkcnMmN9zQr/raw", true))()</textarea>
</div>

<div class="footer">Last updated: January 2026</div>

<script>
const total={brainrot:5,blox:5,other:2};
let prog={brainrot:0,blox:0,other:0};

function step(page,btn,link){
if(btn.dataset.done)return;
btn.dataset.done=1;btn.style.opacity=.6;prog[page]++;
let p=Math.floor(prog[page]/total[page]*100);
document.getElementById("bar"+cap(page)).style.width=p+"%";
document.getElementById("percent"+cap(page)).innerText=p+"%";
if(p===100)document.getElementById(page+"Scripts").style.display="block";
window.open(link,"_blank");
}
function copy(btn){
if(confirm("Use The Script In Second Sea Cafe Or It Won’t Work\n\nPress OK to confirm")){
navigator.clipboard.writeText(btn.previousElementSibling.value);
alert("Copied!");
}
}
function openDev(page){
if(prompt("Enter Dev Code")!=="NinjaBlender223")return;
prog[page]=total[page];
document.getElementById("bar"+cap(page)).style.width="100%";
document.getElementById("percent"+cap(page)).innerText="100%";
document.getElementById(page+"Scripts").style.display="block";
devPanel.style.display="block";
}
function switchPage(){brainrotPage.style.display="none";bloxPage.style.display="block"}
function showOther(){bloxPage.style.display="none";otherPage.style.display="block"}
function backHome(){otherPage.style.display="none";brainrotPage.style.display="block"}
function cap(x){return x.charAt(0).toUpperCase()+x.slice(1)}
</script>

</body>
</html>
