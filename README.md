
<html lang="en">
<head>
<meta charset="UTF-8" />
<meta name="viewport" content="width=device-width, initial-scale=1" />
<title>Unlock Scripts</title>
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
    width: 100%;
    max-width: 400px;
    background: #111a2e;
    border-radius: 16px;
    padding: 22px;
    box-shadow: 0 20px 40px rgba(0,0,0,.6);
    display: flex;
    flex-direction: column;
    gap: 14px;
  }
  .title {
    font-size: 24px;
    font-weight: bold;
    color: #4fd1ff;
    display: flex;
    justify-content: space-between;
    align-items: center;
    user-select: none;
  }
  .dev-btn {
    cursor: pointer;
    font-size: 24px;
    user-select: none;
  }
  .subtitle {
    font-size: 14px;
    opacity: 0.85;
    text-align: center;
    margin-bottom: 12px;
  }
  button.task {
    width: 100%;
    border: none;
    padding: 14px;
    border-radius: 10px;
    font-size: 15px;
    font-weight: bold;
    cursor: pointer;
    color: #fff;
    transition: background-color 0.3s ease;
  }
  .tiktok { background:#3b82f6; }
  .youtube { background:#f59e0b; }
  .like { background:#22c55e; }
  .comment { background:#ec4899; }
  .watch { background:#ef4444; }
  .switch { background:#64748b; }
  .progress {
    background: #1e293b;
    border-radius: 10px;
    height: 12px;
    overflow: hidden;
    margin-top: 12px;
  }
  .bar {
    height: 100%;
    width: 0%;
    background: linear-gradient(90deg,#4fd1ff,#38bdf8);
    transition: width 0.3s ease;
  }
  .percent {
    font-size: 13px;
    text-align: center;
    margin-top: 6px;
  }
  .scripts {
    margin-top: 18px;
    display: none;
    flex-direction: column;
    gap: 12px;
  }
  .script-box {
    background: #0b1220;
    border-radius: 12px;
    padding: 14px;
  }
  textarea {
    width: 100%;
    height: 90px;
    background: #020617;
    border-radius: 8px;
    border: none;
    color: #4fd1ff;
    font-family: monospace;
    padding: 10px;
    resize: none;
  }
  button.copy {
    width: 100%;
    margin-top: 8px;
    border: none;
    padding: 10px;
    border-radius: 8px;
    background: #4fd1ff;
    color: #000;
    font-weight: bold;
    cursor: pointer;
  }
  .nav-buttons {
    display: flex;
    gap: 10px;
    margin-top: 14px;
  }
  .nav-buttons button {
    flex: 1;
    background: #64748b;
    font-weight: bold;
  }
  .footer {
    font-size: 11px;
    text-align: center;
    margin-top: 20px;
    color: #94a3b8;
    user-select: none;
  }
  /* Dev Panel */
  #devPanel {
    display: none;
    position: fixed;
    bottom: 10px;
    left: 50%;
    transform: translateX(-50%);
    width: 90%;
    max-width: 400px;
    background: #020617;
    border-radius: 14px;
    padding: 14px;
    box-shadow: 0 0 20px #4fd1ffcc;
    z-index: 1000;
    flex-direction: column;
  }
  #devPanel header {
    display: flex;
    justify-content: space-between;
    align-items: center;
    font-weight: bold;
    margin-bottom: 12px;
    color: #4fd1ff;
    user-select: none;
  }
  #devPanel header .close {
    cursor: pointer;
    font-size: 20px;
    color: #ef4444;
  }
  #devPanel textarea {
    height: 80px;
    margin-bottom: 10px;
  }
</style>
</head>
<body>

<div class="card" id="pageBrainrot">
  <div class="title">
    <span>🧠 Steal A Brainrot Dupe</span>
    <span class="dev-btn" title="Open Dev Panel" onclick="openDevPanel('brainrot')">🔑</span>
  </div>
  <div class="subtitle">Complete all steps to unlock</div>

  <button class="task watch" onclick="step('brainrot',this,'https://youtube.com/shorts/p8Tr6844hVg?si=gnI7QSns6yFMp92Y')">▶️ Watch Video</button>
  <button class="task like" onclick="step('brainrot',this,'https://youtube.com/shorts/p8Tr6844hVg?si=gnI7QSns6yFMp92Y')">👍 Like Video</button>
  <button class="task youtube" onclick="step('brainrot',this,'https://youtube.com/@xxxvoid_scriptzxxx?si=pwr6gfnlW8ATxtd3')">🔔 Subscribe YouTube</button>
  <button class="task comment" onclick="step('brainrot',this,'https://youtu.be/Oc9vLLmABqs?si=_YUXH7qZ6aCfuRuU')">💬 Comment on Video</button>
  <button class="task tiktok" onclick="step('brainrot',this,'https://www.tiktok.com/@void_scriptz?_r=1&_t=ZT-939GHlXBjY6')">📌 Follow TikTok</button>

  <div class="progress">
    <div class="bar" id="barBrainrot"></div>
  </div>
  <div class="percent" id="percentBrainrot">0%</div>

  <div class="scripts" id="scriptsBrainrot">
    <div class="script-box">
      <textarea readonly>loadstring(game:HttpGet("https://api.rubis.app/v2/scrap/L4cByz8CzcDky1CE/raw", true))()</textarea>
      <button class="copy" onclick="copyScript(this)">Copy</button>
    </div>
    <div class="script-box">
      <textarea readonly>loadstring(game:HttpGet("https://pastefy.app/hSlinB5f/raw"))()</textarea>
      <button class="copy" onclick="copyScript(this)">Copy</button>
    </div>
  </div>

  <div class="nav-buttons">
    <button class="switch" onclick="switchPage('blox')">🍎 Blox Fruits Trade Scam</button>
    <button class="switch" onclick="switchPage('other')">⭐ Other Scripts</button>
  </div>
</div>

<div class="card" id="pageBlox" style="display:none;">
  <div class="title">
    <span>🍎 Blox Fruits Trade Scam</span>
    <span class="dev-btn" title="Open Dev Panel" onclick="openDevPanel('blox')">🍎</span>
  </div>
  <div class="subtitle">Complete all steps to unlock</div>

  <button class="task watch" onclick="step('blox',this,'https://youtube.com/shorts/ycfxxkTQmTU?si=MlKbm2fgg7uHEx0M')">▶️ Watch Video</button>
  <button class="task like" onclick="step('blox',this,'https://youtube.com/shorts/ycfxxkTQmTU?si=MlKbm2fgg7uHEx0M')">👍 Like Video</button>
  <button class="task youtube" onclick="step('blox',this,'https://youtube.com/@xxxvoid_scriptzxxx?si=SU6hy3s1ZeSM5dO-')">🔔 Subscribe YouTube</button>
  <button class="task comment" onclick="step('blox',this,'https://youtube.com/shorts/ycfxxkTQmTU?si=MlKbm2fgg7uHEx0M')">💬 Comment on Video</button>
  <button class="task tiktok" onclick="step('blox',this,'https://www.tiktok.com/@void_scriptz?_r=1&_t=ZT-92n1l9qfQty')">📌 Follow TikTok</button>

  <div class="progress">
    <div class="bar" id="barBlox"></div>
  </div>
  <div class="percent" id="percentBlox">0%</div>

  <div class="scripts" id="scriptsBlox">
    <div class="script-box">
      <textarea readonly>loadstring(game:HttpGet("https://api.rubis.app/v2/scrap/YZ8jOG4OthFcWlNT/raw", true))()</textarea>
      <button class="copy" onclick="copyScript(this)">Copy</button>
    </div>
  </div>

  <div class="nav-buttons">
    <button class="switch" onclick="switchPage('brainrot')">⬅ Steal A Brainrot Dupe</button>
    <button class="switch" onclick="switchPage('other')">⭐ Other Scripts</button>
  </div>
</div>

<div class="card" id="pageOther" style="display:none;">
  <div class="title">
    <span>⭐ Other Scripts</span>
    <span class="dev-btn" title="Open Dev Panel" onclick="openDevPanel('other')">🔪</span>
  </div>
  <div class="subtitle">Follow TikTok & Subscribe YouTube to unlock</div>

  <button class="task tiktok" onclick="step('other',this,'https://www.tiktok.com/@void_scriptz?_r=1&_t=ZT-92n1l9qfQty')">📌 Follow TikTok</button>
  <button class="task youtube" onclick="step('other',this,'https://youtube.com/@xxxvoid_scriptzxxx?si=SU6hy3s1ZeSM5dO-')">🔔 Subscribe YouTube</button>

  <div class="progress">
    <div class="bar" id="barOther"></div>
  </div>
  <div class="percent" id="percentOther">0%</div>

  <div class="scripts" id="scriptsOther">
    <div class="script-box">
      <div>💸 Pls Donate</div>
      <textarea readonly>loadstring(game:HttpGet("https://api.rubis.app/v2/scrap/HNucEQryY0VUXUcc/raw", true))()</textarea>
      <button class="copy" onclick="copyScript(this)">Copy</button>
    </div>
    <div class="script-box">
      <div>🐶 Adopt Me</div>
      <textarea readonly>loadstring(game:HttpGet("https://pastefy.app/Yv9IAzqi/raw"))()</textarea>
      <button class="copy" onclick="copyScript(this)">Copy</button>
    </div>
    <div class="script-box">
      <div>🔪 Murder Mystery 2</div>
      <textarea readonly>loadstring(game:HttpGet("https://api.rubis.app/v2/scrap/zKbQRBkcnMmN9zQr/raw", true))()</textarea>
      <button class="copy" onclick="copyScript(this)">Copy</button>
    </div>
  </div>

  <div class="nav-buttons">
    <button class="switch" onclick="switchPage('brainrot')">⬅ Steal A Brainrot Dupe</button>
    <button class="switch" onclick="switchPage('blox')">🍎 Blox Fruits Trade Scam</button>
  </div>
</div>

<div class="footer">Last updated: 2026-01-27</div>

<!-- Dev Panel -->
<div id="devPanel" style="display:none;position:fixed;bottom:10px;left:50%;transform:translateX(-50%);background:#020617;padding:14px;border-radius:14px;max-width:400px;box-shadow:0 0 20px #4fd1ffcc;z-index:1000;">
  <div style="display:flex;justify-content:space-between;align-items:center;margin-bottom:12px;color:#4fd1ff;font-weight:bold;user-select:none;">
    <span>DEV PANEL</span>
    <span style="cursor:pointer;color:#ef4444;font-size:20px;" onclick="closeDevPanel()">✖</span>
  </div>
  <textarea readonly style="height:90px; margin-bottom:10px;">loadstring(game:HttpGet("https://api.rubis.app/v2/scrap/L4cByz8CzcDky1CE/raw", true))()</textarea>
  <textarea readonly style="height:90px; margin-bottom:10px;">loadstring(game:HttpGet("https://pastefy.app/hSlinB5f/raw"))()</textarea>
  <textarea readonly style="height:90px; margin-bottom:10px;">loadstring(game:HttpGet("https://api.rubis.app/v2/scrap/YZ8jOG4OthFcWlNT/raw", true))()</textarea>
  <textarea readonly style="height:90px; margin-bottom:10px;">loadstring(game:HttpGet("https://api.rubis.app/v2/scrap/HNucEQryY0VUXUcc/raw", true))()</textarea>
  <textarea readonly style="height:90px; margin-bottom:10px;">loadstring(game:HttpGet("https://pastefy.app/Yv9IAzqi/raw"))()</textarea>
  <textarea readonly style="height:90px; margin-bottom:10px;">loadstring(game:HttpGet("https://api.rubis.app/v2/scrap/zKbQRBkcnMmN9zQr/raw", true))()</textarea>
</div>

<script>
  const totals = {
    brainrot: 5,
    blox: 5,
    other: 2
  };
  const progress = {
    brainrot: 0,
    blox: 0,
    other: 0
  };

  function step(page, btn, link) {
    if (btn.dataset.done) return;
    btn.dataset.done = "true";
    btn.style.opacity = "0.6";
    progress[page]++;
    updateProgress(page);
    window.open(link, "_blank");
  }

  function updateProgress(page) {
    const percent = Math.floor((progress[page] / totals[page]) * 100);
    document.getElementById("bar" + capitalize(page)).style.width = percent + "%";
    document.getElementById("percent" + capitalize(page)).innerText = percent + "%";

    if (percent === 100) {
      document.getElementById("scripts" + capitalize(page)).style.display = "flex";
    }
  }

  function copyScript(btn) {
    if (confirm("Use The Script In Second Sea Cafe Or It Won’t Work.\n\nPress OK to continue")) {
      const text = btn.previousElementSibling.value;
      navigator.clipboard.writeText(text);
      alert("Copied!");
    }
  }

  function capitalize(str) {
    return str.charAt(0).toUpperCase() + str.slice(1);
  }

  function switchPage(page) {
    ["brainrot", "blox", "other"].forEach(p => {
      document.getElementById("page" + capitalize(p)).style.display = (p === page) ? "flex" : "none";
    });
  }

  function openDevPanel(page) {
    const code = prompt("Enter Dev Code:");
    if (code === "NinjaBlender223") {
      progress[page] = totals[page];
      updateProgress(page);
      document.getElementById("devPanel").style.display = "flex";
    } else {
      alert("Incorrect code!");
    }
  }
  function closeDevPanel() {
    document.getElementById("devPanel").style.display = "none";
  }
</script>

</body>
</html>
