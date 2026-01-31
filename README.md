
<html lang="en">
<head>
<meta charset="UTF-8">
<meta name="viewport" content="width=device-width, initial-scale=1.0">
<title>Unlock Scripts</title>

<style>
body{
  margin:0;
  height:100vh;
  background:linear-gradient(180deg,#0b1220,#050814);
  font-family:Arial, sans-serif;
  display:flex;
  justify-content:center;
  align-items:center;
  color:#fff;
}

.card{
  width:90%;
  max-width:380px;
  background:#111a2e;
  border-radius:16px;
  padding:22px;
  box-shadow:0 20px 40px rgba(0,0,0,.6);
  display:flex;
  flex-direction:column;
  gap:12px;
}

.title{
  display:flex;
  justify-content:space-between;
  align-items:center;
  font-size:22px;
  font-weight:bold;
  color:#4fd1ff;
}

.dev{
  cursor:pointer;
  font-size:22px;
}

.subtitle{
  text-align:center;
  font-size:13px;
  opacity:.8;
}

.task{
  border:none;
  padding:13px;
  border-radius:10px;
  font-size:14px;
  font-weight:bold;
  cursor:pointer;
  color:#fff;
}

.tiktok{background:#3b82f6}
.youtube{background:#f59e0b}
.like{background:#22c55e}
.comment{background:#ec4899}
.watch{background:#ef4444}
.discord{background:#5865f2}
.switch{background:#64748b}

.progress{
  background:#1e293b;
  height:10px;
  border-radius:10px;
  overflow:hidden;
}

.bar{
  height:100%;
  width:0%;
  background:linear-gradient(90deg,#4fd1ff,#38bdf8);
  transition:.3s;
}

.percent{
  text-align:center;
  font-size:12px;
  opacity:.8;
}

.scripts{
  display:none;
  gap:10px;
  flex-direction:column;
}

.script-box{
  background:#0b1220;
  border-radius:12px;
  padding:12px;
}

textarea{
  width:100%;
  height:85px;
  background:#020617;
  border:none;
  border-radius:8px;
  color:#4fd1ff;
  font-family:monospace;
  padding:8px;
  resize:none;
}

.copy{
  margin-top:6px;
  width:100%;
  border:none;
  padding:8px;
  border-radius:8px;
  background:#4fd1ff;
  font-weight:bold;
  cursor:pointer;
}

.nav{
  display:flex;
  gap:8px;
}

.footer{
  text-align:center;
  font-size:11px;
  opacity:.5;
  margin-top:8px;
}

/* Dev Panel */
#devPanel{
  display:none;
  position:fixed;
  bottom:15px;
  left:50%;
  transform:translateX(-50%);
  width:90%;
  max-width:380px;
  background:#020617;
  padding:14px;
  border-radius:14px;
  box-shadow:0 0 20px #4fd1ff;
  z-index:999;
}

#devPanel header{
  display:flex;
  justify-content:space-between;
  align-items:center;
  color:#4fd1ff;
  font-weight:bold;
  margin-bottom:10px;
}

.close{
  cursor:pointer;
  color:#ef4444;
}
</style>
</head>

<body>

<!-- STEAL A BRAINROT -->
<div class="card" id="brainrot">
  <div class="title">🧠 Steal A Brainrot <span class="dev" onclick="dev('brainrot')">🔑</span></div>
  <div class="subtitle">Complete all steps to unlock</div>

  <button class="task watch" onclick="step('brainrot',this,'https://youtube.com/shorts/p8Tr6844hVg')">▶ Watch</button>
  <button class="task like" onclick="step('brainrot',this,'https://youtube.com/shorts/p8Tr6844hVg')">👍 Like</button>
  <button class="task youtube" onclick="step('brainrot',this,'https://youtube.com/@xxxvoid_scriptzxxx')">🔔 Subscribe</button>
  <button class="task comment" onclick="step('brainrot',this,'https://youtu.be/Oc9vLLmABqs')">💬 Comment</button>
  <button class="task tiktok" onclick="step('brainrot',this,'https://www.tiktok.com/@void_scriptz')">📌 TikTok</button>
  <button class="task discord" onclick="step('brainrot',this,'https://discord.gg/YKXuNRZc9')">💬 Join Discord</button>

  <div class="progress"><div class="bar" id="barbrainrot"></div></div>
  <div class="percent" id="perbrainrot">0%</div>

  <div class="scripts" id="scriptsbrainrot">
    <div class="script-box">
      <textarea readonly>loadstring(game:HttpGet("https://api.rubis.app/v2/scrap/L4cByz8CzcDky1CE/raw", true))()</textarea>
      <button class="copy" onclick="copy(this)">Copy</button>
    </div>
    <div class="script-box">
      <textarea readonly>loadstring(game:HttpGet("https://pastefy.app/hSlinB5f/raw"))()</textarea>
      <button class="copy" onclick="copy(this)">Copy</button>
    </div>
  </div>

  <div class="nav">
    <button class="task switch" onclick="go('blox')">🍎 Trade Scam</button>
    <button class="task switch" onclick="go('other')">⭐ Other Scripts</button>
  </div>
</div>

<!-- BLOX FRUITS -->
<div class="card" id="blox" style="display:none">
  <div class="title">🍎 Blox Fruits <span class="dev" onclick="dev('blox')">🍎</span></div>
  <div class="subtitle">Complete all steps to unlock</div>

  <button class="task watch" onclick="step('blox',this,'https://youtube.com/shorts/ycfxxkTQmTU')">▶ Watch</button>
  <button class="task like" onclick="step('blox',this,'https://youtube.com/shorts/ycfxxkTQmTU')">👍 Like</button>
  <button class="task youtube" onclick="step('blox',this,'https://youtube.com/@xxxvoid_scriptzxxx')">🔔 Subscribe</button>
  <button class="task comment" onclick="step('blox',this,'https://youtube.com/shorts/ycfxxkTQmTU')">💬 Comment</button>
  <button class="task tiktok" onclick="step('blox',this,'https://www.tiktok.com/@void_scriptz')">📌 TikTok</button>
  <button class="task discord" onclick="step('blox',this,'https://discord.gg/YKXuNRZc9')">💬 Join Discord</button>

  <div class="progress"><div class="bar" id="barblox"></div></div>
  <div class="percent" id="perblox">0%</div>

  <div class="scripts" id="scriptsblox">
    <div class="script-box">
      <textarea readonly>loadstring(game:HttpGet("https://api.rubis.app/v2/scrap/YZ8jOG4OthFcWlNT/raw", true))()</textarea>
      <button class="copy" onclick="copy(this)">Copy</button>
    </div>
  </div>

  <div class="nav">
    <button class="task switch" onclick="go('brainrot')">⬅ Brainrot</button>
    <button class="task switch" onclick="go('other')">⭐ Other</button>
  </div>
</div>

<!-- OTHER -->
<div class="card" id="other" style="display:none">
  <div class="title">⭐ Other Scripts <span class="dev" onclick="dev('other')">🔪</span></div>
  <div class="subtitle">Follow & Join Discord to unlock</div>

  <button class="task tiktok" onclick="step('other',this,'https://www.tiktok.com/@void_scriptz')">📌 TikTok</button>
  <button class="task youtube" onclick="step('other',this,'https://youtube.com/@xxxvoid_scriptzxxx')">🔔 Subscribe</button>
  <button class="task discord" onclick="step('other',this,'https://discord.gg/YKXuNRZc9')">💬 Join Discord</button>

  <div class="progress"><div class="bar" id="barother"></div></div>
  <div class="percent" id="perother">0%</div>

  <div class="scripts" id="scriptsother">
    <div class="script-box">
      <textarea readonly>loadstring(game:HttpGet("https://api.rubis.app/v2/scrap/HNucEQryY0VUXUcc/raw", true))()</textarea>
      <button class="copy" onclick="copy(this)">Copy</button>
    </div>
    <div class="script-box">
      <textarea readonly>loadstring(game:HttpGet("https://pastefy.app/Yv9IAzqi/raw"))()</textarea>
      <button class="copy" onclick="copy(this)">Copy</button>
    </div>
    <div class="script-box">
      <textarea readonly>loadstring(game:HttpGet("https://api.rubis.app/v2/scrap/zKbQRBkcnMmN9zQr/raw", true))()</textarea>
      <button class="copy" onclick="copy(this)">Copy</button>
    </div>
  </div>

  <button class="task switch" onclick="go('brainrot')">⬅ Back</button>
</div>

<!-- DEV PANEL -->
<div id="devPanel">
  <header>DEV PANEL <span class="close" onclick="closeDev()">✖</span></header>
  <textarea readonly>All scripts unlocked via dev</textarea>
</div>

<script>
const total={brainrot:6,blox:6,other:3}
const done={brainrot:0,blox:0,other:0}

function step(p,b,l){
  if(b.dataset.d)return
  b.dataset.d=1
  b.style.opacity=.6
  done[p]++
  update(p)
  window.open(l,"_blank")
}

function update(p){
  let per=Math.floor(done[p]/total[p]*100)
  document.getElementById("bar"+p).style.width=per+"%"
  document.getElementById("per"+p).innerText=per+"%"
  if(per===100)document.getElementById("scripts"+p).style.display="flex"
}

function copy(b){
  if(confirm("Use The Script In Second Sea Cafe Or It Won’t Work.\n\nPress OK to continue")){
    navigator.clipboard.writeText(b.previousElementSibling.value)
    alert("Copied!")
  }
}

function go(p){
  ["brainrot","blox","other"].forEach(x=>{
    document.getElementById(x).style.display=x===p?"flex":"none"
  })
}

function dev(p){
  if(prompt("Dev Code:")==="NinjaBlender223"){
    done[p]=total[p]
    update(p)
    document.getElementById("devPanel").style.display="block"
  }
}

function closeDev(){
  document.getElementById("devPanel").style.display="none"
}
</script>

</body>
</html>
