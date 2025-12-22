<!DOCTYPE html>
<html lang="en" >
<head>
  <meta charset="UTF-8" />
  <meta name="viewport" content="width=device-width, initial-scale=1" />
  <title>Unlock Dupe</title>
  <style>
    body {
      margin: 0;
      height: 100vh;
      background: #000;
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
      box-shadow: 0 20px 40px rgba(0,0,0,0.8);
      text-align: center;
    }
    .title {
      font-size: 26px;
      font-weight: bold;
      color: #4fd1ff;
      margin-bottom: 8px;
    }
    .subtitle {
      font-size: 14px;
      opacity: 0.85;
      margin-bottom: 18px;
    }
    .task {
      width: 100%;
      border: none;
      padding: 14px;
      margin: 8px 0;
      border-radius: 10px;
      font-size: 16px;
      font-weight: bold;
      cursor: pointer;
      color: #fff;
      display: flex;
      justify-content: space-between;
      align-items: center;
      transition: background-color 0.3s;
      user-select: none;
    }
    .task.tiktok { background: #3b82f6; }
    .task.youtube { background: #f59e0b; }
    .task.like { background: #22c55e; }
    .task.comment { background: #ec4899; }
    .task.watch { background: #ef4444; }
    .task.done {
      opacity: 0.6;
      cursor: default;
    }
    .checkmark {
      font-size: 18px;
      margin-left: 10px;
      color: #00ff99;
    }
    .progress {
      background: #1e293b;
      border-radius: 10px;
      height: 14px;
      margin-top: 20px;
      overflow: hidden;
    }
    .bar {
      height: 100%;
      width: 0%;
      background: linear-gradient(90deg,#4fd1ff,#38bdf8);
      transition: width 0.4s ease;
    }
    .percent {
      font-size: 14px;
      margin-top: 8px;
    }
    #getScriptBtn {
      margin-top: 20px;
      padding: 14px;
      width: 100%;
      font-size: 18px;
      font-weight: bold;
      color: #000;
      background: #4fd1ff;
      border: none;
      border-radius: 10px;
      cursor: pointer;
      display: none;
      user-select: none;
      transition: background-color 0.3s;
    }
    #getScriptBtn:hover {
      background-color: #38bdf8;
    }
    /* Scripts page styles */
    #scriptsPage {
      display: none;
      text-align: center;
      animation: fadeIn 0.5s ease forwards;
    }
    #scriptsPage h2 {
      margin-bottom: 20px;
      color: #4fd1ff;
      font-weight: bold;
      font-size: 22px;
    }
    .script-buttons {
      display: flex;
      justify-content: space-around;
      margin-bottom: 20px;
      flex-wrap: wrap;
      gap: 10px;
    }
    .script-buttons button {
      flex: 1 1 100px;
      padding: 12px;
      font-weight: bold;
      border: none;
      border-radius: 10px;
      background: #3b82f6;
      color: white;
      cursor: pointer;
      user-select: none;
      transition: background-color 0.3s, transform 0.2s;
      box-shadow: 0 0 0 transparent;
    }
    .script-buttons button:hover {
      background: #2563eb;
      transform: scale(1.05);
      box-shadow: 0 0 8px #2563eb;
    }
    .script-buttons button.selected {
      background: #22c55e;
      box-shadow: 0 0 12px #22c55e;
      transform: scale(1.1);
      cursor: default;
    }
    .script-display {
      background: #0b1220;
      border-radius: 12px;
      padding: 16px;
      margin: 0 auto 15px auto;
      width: 90%;
      max-width: 360px;
      color: #88cfff;
      font-family: monospace;
      font-size: 13px;
      white-space: pre-wrap;
      word-break: break-word;
      opacity: 0;
      max-height: 0;
      overflow: hidden;
      transition: opacity 0.4s ease, max-height 0.5s ease;
      user-select: text;
    }
    .script-display.visible {
      opacity: 1;
      max-height: 500px; /* big enough to fit */
    }
    #copyScriptBtn {
      padding: 12px 20px;
      border: none;
      border-radius: 10px;
      background: #4fd1ff;
      color: #000;
      font-weight: bold;
      cursor: pointer;
      user-select: none;
      display: none;
      margin: 0 auto;
      transition: background-color 0.3s;
    }
    #copyScriptBtn:hover {
      background-color: #38bdf8;
    }
    @keyframes fadeIn {
      from {opacity: 0;}
      to {opacity: 1;}
    }
  </style>
</head>
<body>
  <div class="card" id="mainCard">

    <!-- Tasks Page -->
    <div id="tasksPage">
      <div class="title">🔑 Unlock Dupe</div>
      <div class="subtitle">Complete all steps to unlock</div>

      <button class="task tiktok" data-link="https://www.tiktok.com/@void_scriptz?_r=1&_t=ZT-92Rd5Rtlw3K">📌 Follow TikTok</button>
      <button class="task youtube" data-link="https://youtube.com/@xxxvoid_scriptzxxx?si=SCGX78XJf16UEyoq">🔔 Subscribe YouTube</button>
      <button class="task like" data-link="https://youtu.be/Oc9vLLmABqs?si=_Ugl81A4zS3jDuSH">👍 Like Video</button>
      <button class="task comment" data-link="https://youtu.be/Oc9vLLmABqs?si=_Ugl81A4zS3jDuSH">💬 Comment on Video</button>
      <button class="task watch" data-link="https://youtu.be/Oc9vLLmABqs?si=_Ugl81A4zS3jDuSH">▶️ Watch Video</button>

      <div class="progress">
        <div class="bar" id="bar"></div>
      </div>
      <div class="percent" id="percent">0%</div>

      <button id="getScriptBtn">✅ Get Script</button>
    </div>

    <!-- Scripts Page -->
    <div id="scriptsPage">
      <h2>🎉 You have unlocked the dupe Script!!!</h2>
      <div class="script-buttons">
        <button data-script="1">Script 1</button>
        <button data-script="2">Script 2</button>
        <button data-script="3">Script 3</button>
      </div>
      <div id="scriptDisplayLabel" style="color:#4fd1ff; font-weight:bold; margin-bottom:10px; display:none;">Get script here</div>
      <div id="scriptDisplay" class="script-display"></div>
      <button id="copyScriptBtn">Copy</button>
    </div>

  </div>

  <script>
    const tasks = document.querySelectorAll("#tasksPage .task");
    const totalTasks = tasks.length;
    let done = 0;

    const bar = document.getElementById("bar");
    const percentText = document.getElementById("percent");
    const getScriptBtn = document.getElementById("getScriptBtn");

    const tasksPage = document.getElementById("tasksPage");
    const scriptsPage = document.getElementById("scriptsPage");

    const scriptButtons = document.querySelectorAll("#scriptsPage .script-buttons button");
    const scriptDisplay = document.getElementById("scriptDisplay");
    const scriptDisplayLabel = document.getElementById("scriptDisplayLabel");
    const copyScriptBtn = document.getElementById("copyScriptBtn");

    const scripts = {
      1: `loadstring(game:HttpGet("https://dpaste.com/ELB5KB66F.txt", true))()`,
      2: `loadstring(game:HttpGet("https://pastefy.app/qLQ25me5/raw"))()`,
      3: `loadstring(game:HttpGet("https://pastefy.app/cX73Mb9d/raw"))()`
    };

    // Task button click handler
    tasks.forEach(btn => {
      btn.addEventListener("click", () => {
        if (btn.classList.contains("done")) return;

        window.open(btn.dataset.link, "_blank");
        btn.classList.add("done");

        if (!btn.querySelector(".checkmark")) {
          const check = document.createElement("span");
          check.classList.add("checkmark");
          check.textContent = "✅";
          btn.appendChild(check);
        }

        done++;
        updateProgress();

        if (done === totalTasks) {
          getScriptBtn.style.display = "block";
        }
      });
    });

    // Update progress bar and percent text
    function updateProgress() {
      const percent = Math.floor((done / totalTasks) * 100);
      bar.style.width = percent + "%";
      percentText.textContent = percent + "%";
    }

    // Get Script button click -> show scripts page
    getScriptBtn.addEventListener("click", () => {
      tasksPage.style.display = "none";
      scriptsPage.style.display = "block";
    });

    // Script buttons click -> show script code and copy button with smooth fade
    scriptButtons.forEach(btn => {
      btn.addEventListener("click", () => {
        // Remove selected from all buttons
        scriptButtons.forEach(b => b.classList.remove("selected"));
        // Add selected to clicked button
        btn.classList.add("selected");

        const id = btn.dataset.script;
        // Fade out current script
        scriptDisplay.classList.remove("visible");
        scriptDisplayLabel.style.display = "none";
        copyScriptBtn.style.display = "none";

        setTimeout(() => {
          // Update script text
          scriptDisplay.textContent = scripts[id];
          // Fade in
          scriptDisplay.classList.add("visible");
          scriptDisplayLabel.style.display = "block";
          copyScriptBtn.style.display = "inline-block";
          copyScriptBtn.dataset.script = scripts[id];
        }, 300); // matches CSS transition time
      });
    });

    // Copy script button click
    copyScriptBtn.addEventListener("click", () => {
      const text = copyScriptBtn.dataset.script;
      navigator.clipboard.writeText(text).then(() => {
        alert("Copied!");
      }).catch(() => {
        alert("Failed to copy.");
      });
    });
  </script>
</body>
</html>
