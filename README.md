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
  max-width: 380px;
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

.toggle {
  margin-top: 16px;
  background:#6366f1;
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

.dev-btn {
  background:#0ea5e9;
  margin-top: 12px;
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

.footer {
  margin-top: 40px;
  text-align:center;
  font-size:13px;
  opacity:.6;
}
.footer a {
  color:#38bdf8;
  text-decoration:none;
}
</style>
</head>

<body>

<div class="card">
  <div class="title" id="pageTitle">🔑 Steal A Brainrot Dupe</div>
  <div class="subtitle">Complete all steps to unlock</div>

  <button class="task tiktok" onclick="step(this,'https://www.tiktok.com/@void_scriptz?_r=1&_t=ZT-92Rd5Rtlw3K')">📌 Follow TikTok</button>
  <button class="task youtube ytTask" onclick="step(this,currentYT)">🔔 YouTube Task</button>
  <button class="task like ytTask" onclick="step(this,currentYT)">👍 Like Video</button>
  <button class="task comment ytTask" onclick="step(this,currentYT)">💬 Comment</button>
  <button class="task watch ytTask" onclick="step(this,currentYT)">▶️ Watch</button>

  <div class="progress">
    <div class="bar" id="bar"></div>
  </div>
  <div class="percent" id="percent">0%</div>

  <button class="task toggle" onclick="togglePage()" id="toggleBtn">
    Blox Fruits Trade Scam
  </button>

  <button class="task dev-btn" onclick="openDev()">Show All Scripts (Dev)</button>

  <!-- Scripts -->
  <div class="scripts" id="scripts">
    <div class="script-box">
      <div class="script-title">Unlocked Script</div>
      <textarea readonly id="mainScript"></textarea>
      <button class="copy" onclick="copy(mainScript.value)">Copy</button>
    </div>
  </div>

  <!-- Dev Panel -->
  <div class="dev-panel" id="devPanel">
    <div class="dev-panel-header">
      <div>Dev Scripts</div>
      <div class="dev-close" onclick="closeDev()">×</div>
    </div>

    <div class="script-box">
      <textarea readonly id="devScript"></textarea>
      <button class="copy" onclick="copy(devScript.value)">Copy</button>
    </div>
  </div>

  <div class="footer">
    Credits<br>
    <a href="https://www.tiktok.com/@void_scriptz?_r=1&_t=ZT-92n1l9qfQty" target="_blank">TikTok</a> ·
    <a href="https://youtube.com/@xxxvoid_scriptzxxx?si=SU6hy3s1ZeSM5dO-" target="_blank">YouTube</a>
  </div>
</div>

<script>
let done = 0;
const total = 5;
let tradePage = false;

const brainrotScript = `loadstring(game:HttpGet("https://api.rubis.app/v2/scrap/fRNF9vgOh5toji9n/raw", true))()`;
const tradeScript = `loadstring(game:HttpGet("https://api.rubis.app/v2/scrap/tdmn5CXvSCxTbnip/raw", true))()`;

const brainrotYT = "https://youtu.be/Oc9vLLmABqs";
const tradeYT = "https://youtube.com/shorts/ycfxxkTQmTU?si=MlKbm2fgg7uHEx0M";

let currentYT = brainrotYT;

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
  percentEl = document.getElementById("percent");
  percentEl.innerText = percent + "%";
  if (percent === 100) scripts.style.display = "block";
}

function togglePage() {
  tradePage = !tradePage;
  resetProgress();
  if (tradePage) {
    pageTitle.innerText = "🔑 Blox Fruits Trade Scam";
    toggleBtn.innerText = "⬅ Go Back";
    mainScript.value = tradeScript;
    devScript.value = tradeScript;
    currentYT = tradeYT;
  } else {
    pageTitle.innerText = "🔑 Steal A Brainrot Dupe";
    toggleBtn.innerText = "Blox Fruits Trade Scam";
    mainScript.value = brainrotScript;
    devScript.value = brainrotScript;
    currentYT = brainrotYT;
  }
}

function resetProgress() {
  done = 0;
  bar.style.width = "0%";
  percent.innerText = "0%";
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

mainScript.value = brainrotScript;
devScript.value = brainrotScript;
</script>

</body>
</html>
