
<!DOCTYPE html>
<html lang="zh-CN">
<head>
  <meta charset="UTF-8" />
  <title>NEURAL · Console</title>
  <style>
    * {
      box-sizing: border-box;
      font-family: "Inter", "PingFang SC", "Microsoft YaHei", sans-serif;
    }

    body {
      margin: 0;
      height: 100vh;
      background: radial-gradient(circle at top, #1b1f2a, #0b0e14);
      display: flex;
      align-items: center;
      justify-content: center;
      color: #e5e7eb;
    }

    .card {
      width: 720px;
      max-width: 90%;
      background: rgba(20, 24, 38, 0.85);
      backdrop-filter: blur(12px);
      border-radius: 18px;
      box-shadow: 0 0 60px rgba(99,102,241,0.15);
      padding: 28px;
    }

    .title {
      font-size: 22px;
      letter-spacing: 2px;
      color: #a5b4fc;
      margin-bottom: 16px;
    }

    .subtitle {
      font-size: 13px;
      opacity: 0.6;
      margin-bottom: 20px;
    }

    .output {
      height: 260px;
      overflow-y: auto;
      padding: 16px;
      background: rgba(0,0,0,0.25);
      border-radius: 12px;
      font-size: 14px;
      line-height: 1.6;
      margin-bottom: 16px;
    }

    .output span {
      color: #22d3ee;
    }

    .input-row {
      display: flex;
      gap: 12px;
    }

    input {
      flex: 1;
      padding: 14px 16px;
      background: #0f1320;
      border: 1px solid #2a2f45;
      border-radius: 10px;
      color: #e5e7eb;
      font-size: 14px;
      outline: none;
    }

    input:focus {
      border-color: #6366f1;
      box-shadow: 0 0 0 1px rgba(99,102,241,0.5);
    }

    button {
      padding: 0 22px;
      border-radius: 10px;
      border: none;
      background: linear-gradient(135deg, #6366f1, #22d3ee);
      color: #020617;
      font-weight: bold;
      cursor: pointer;
    }

    button:hover {
      opacity: 0.9;
    }
  </style>
</head>

<body>
  <div class="card">
    <div class="title">NEURAL · CONSOLE</div>
    <div class="subtitle">Advanced Cognitive Interface · Local Demo</div>

    <div class="output" id="output">
      <span>System</span>：神经接口初始化完成。<br>
      <span>System</span>：等待用户输入……
    </div>

    <div class="input-row">
      <input id="input" placeholder="输入你的问题，假装在调 AI…" />
      <button onclick="send()">EXEC</button>
    </div>
  </div>

  <script>
    const output = document.getElementById("output");
    const input = document.getElementById("input");

    function typeText(text) {
      let i = 0;
      const interval = setInterval(() => {
        output.innerHTML += text.charAt(i);
        output.scrollTop = output.scrollHeight;
        i++;
        if (i >= text.length) clearInterval(interval);
      }, 18);
    }

    function send() {
      const value = input.value.trim();
      if (!value) return;

      output.innerHTML += `<br><br><span>You</span>：${value}<br><span>AI</span>：`;
      input.value = "";

      // 假装 AI 在思考（装B核心）
      setTimeout(() => {
        typeText("这是一个本地神经接口演示页面，用于展示高级人工智能交互体验。");
      }, 500);
    }
  </script>
</body>
</html>
