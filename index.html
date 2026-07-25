```html
<!DOCTYPE html>
<html lang="zh-CN">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>玄机算卦 - 揭示命运奥秘</title>
    <script src="https://cdn.tailwindcss.com"></script>
    <link href="https://fonts.googleapis.com/css2?family=Noto+Serif+SC:wght@300;500;700&family=Ma+Shan+Zheng&display=swap" rel="stylesheet">
    <style>
        /* Custom Styles & Animations */
        :root {
            --gold-primary: #ffd700;
            --gold-dim: #b8860b;
            --dark-bg: #0f172a;
        }

        body {
            font-family: 'Noto Serif SC', serif;
            background-color: #000;
            overflow-x: hidden;
        }

        .font-artistic {
            font-family: 'Ma Shan Zheng', cursive;
        }

        /* Background Animation */
        .bg-gradient-animate {
            background: linear-gradient(-45deg, #0f0c29, #302b63, #24243e, #000000);
            background-size: 400% 400%;
            animation: gradientBG 15s ease infinite;
        }

        @keyframes gradientBG {
            0% { background-position: 0% 50%; }
            50% { background-position: 100% 50%; }
            100% { background-position: 0% 50%; }
        }

        /* Glassmorphism */
        .glass-panel {
            background: rgba(255, 255, 255, 0.05);
            backdrop-filter: blur(10px);
            -webkit-backdrop-filter: blur(10px);
            border: 1px solid rgba(255, 215, 0, 0.2);
            box-shadow: 0 8px 32px 0 rgba(0, 0, 0, 0.37);
        }

        /* Gold Text Glow */
        .text-glow {
            text-shadow: 0 0 10px rgba(255, 215, 0, 0.5), 0 0 20px rgba(255, 215, 0, 0.3);
        }

        /* Input Styling */
        .input-field {
            background: rgba(0, 0, 0, 0.3);
            border: 1px solid rgba(255, 215, 0, 0.3);
            color: #ffd700;
            transition: all 0.3s ease;
        }
        .input-field:focus {
            border-color: #ffd700;
            box-shadow: 0 0 15px rgba(255, 215, 0, 0.2);
            outline: none;
        }

        /* Button Hover */
        .btn-gold {
            background: linear-gradient(45deg, #b8860b, #ffd700, #b8860b);
            background-size: 200% auto;
            transition: 0.5s;
        }
        .btn-gold:hover {
            background-position: right center;
            box-shadow: 0 0 20px rgba(255, 215, 0, 0.6);
            transform: translateY(-2px);
        }

        /* Modal Animation */
        .modal-enter {
            opacity: 0;
            transform: scale(0.9);
        }
        .modal-enter-active {
            opacity: 1;
            transform: scale(1);
            transition: opacity 300ms, transform 300ms cubic-bezier(0.4, 0, 0.2, 1);
        }
        .modal-exit {
            opacity: 1;
            transform: scale(1);
        }
        .modal-exit-active {
            opacity: 0;
            transform: scale(0.9);
            transition: opacity 200ms, transform 200ms;
        }

        /* Loading Spinner */
        .taiji-loader {
            width: 60px;
            height: 60px;
            border-radius: 50%;
            background: linear-gradient(to bottom, #000 50%, #fff 50%);
            border: 2px solid #ffd700;
            position: relative;
            animation: spin 1s linear infinite;
            box-shadow: 0 0 15px #ffd700;
        }
        .taiji-loader::before, .taiji-loader::after {
            content: '';
            position: absolute;
            width: 20px;
            height: 20px;
            border-radius: 50%;
            left: 50%;
            transform: translateX(-50%);
        }
        .taiji-loader::before {
            top: 10px;
            background: #fff;
            border: 5px solid #000;
        }
        .taiji-loader::after {
            bottom: 10px;
            background: #000;
            border: 5px solid #fff;
        }
        @keyframes spin { 100% { transform: rotate(360deg); } }

        /* Trigram Lines */
        .trigram-line {
            height: 8px;
            background: #ffd700;
            margin-bottom: 6px;
            border-radius: 2px;
            box-shadow: 0 0 5px rgba(255, 215, 0, 0.5);
        }
        .trigram-line.broken {
            display: flex;
            justify-content: space-between;
            background: transparent;
        }
        .trigram-line.broken span {
            width: 48%;
            height: 100%;
            background: #ffd700;
            display: block;
            border-radius: 2px;
            box-shadow: 0 0 5px rgba(255, 215, 0, 0.5);
        }
    </style>
</head>
<body class="bg-gradient-animate min-h-screen flex items-center justify-center text-gray-200 relative">

    <!-- Canvas for subtle particle effects -->
    <canvas id="particleCanvas" class="absolute top-0 left-0 w-full h-full pointer-events-none z-0"></canvas>

    <!-- Main Container -->
    <main class="relative z-10 w-full max-w-md p-6">
        
        <!-- Header -->
        <div class="text-center mb-8 animate-fade-in-down">
            <h1 class="text-6xl font-artistic text-glow text-yellow-400 mb-2 tracking-widest">玄机算卦</h1>
            <p class="text-yellow-200/70 text-sm tracking-[0.2em] uppercase">输入您的信息，揭示命运奥秘</p>
        </div>

        <!-- Form Card -->
        <div class="glass-panel rounded-2xl p-8 shadow-2xl transform transition-all hover:shadow-yellow-900/20">
            <form id="divinationForm" class="space-y-6">
                
                <!-- Name Input -->
                <div class="group">
                    <label class="block text-yellow-500/80 text-xs font-bold mb-2 uppercase tracking-wider">您的姓氏</label>
                    <input type="text" id="userName" required placeholder="请输入姓氏（如：李）" 
                           class="input-field w-full px-4 py-3 rounded-lg text-center text-lg placeholder-yellow-700/50">
                </div>

                <!-- Date Input -->
                <div class="group">
                    <label class="block text-yellow-500/80 text-xs font-bold mb-2 uppercase tracking-wider">出生日期</label>
                    <input type="date" id="birthDate" required 
                           class="input-field w-full px-4 py-3 rounded-lg text-center text-lg [color-scheme:dark]">
                </div>

                <!-- Time Select -->
                <div class="group">
                    <label class="block text-yellow-500/80 text-xs font-bold mb-2 uppercase tracking-wider">出生时辰</label>
                    <div class="relative">
                        <select id="birthTime" class="input-field w-full px-4 py-3 rounded-lg text-center text-lg appearance-none cursor-pointer">
                            <option value="" disabled selected>选择时辰</option>
                            <option value="0">子时 (23:00-01:00)</option>
                            <option value="1">丑时 (01:00-03:00)</option>
                            <option value="2">寅时 (03:00-05:00)</option>
                            <option value="3">卯时 (05:00-07:00)</option>
                            <option value="4">辰时 (07:00-09:00)</option>
                            <option value="5">巳时 (09:00-11:00)</option>
                            <option value="6">午时 (11:00-13:00)</option>
                            <option value="7">未时 (13:00-15:00)</option>
                            <option value="8">申时 (15:00-17:00)</option>
                            <option value="9">酉时 (17:00-19:00)</option>
                            <option value="10">戌时 (19:00-21:00)</option>
                            <option value="11">亥时 (21:00-23:00)</option>
                        </select>
                        <div class="pointer-events-none absolute inset-y-0 right-0 flex items-center px-4 text-yellow-500">
                            <svg class="fill-current h-4 w-4" xmlns="http://www.w3.org/2000/svg" viewBox="0 0 20 20"><path d="M9.293 12.95l.707.707L15.657 8l-1.414-1.414L10 10.828 5.757 6.586 4.343 8z"/></svg>
                        </div>
                    </div>
                </div>

                <!-- Submit Button -->
                <button type="submit" class="btn-gold w-full text-gray-900 font-bold py-4 rounded-lg shadow-lg transform transition-transform active:scale-95 mt-4 text-lg tracking-widest">
                    立即算卦
                </button>
            </form>
        </div>

        <!-- Footer -->
        <div class="text-center mt-8 text-white/20 text-xs">
            <p> 玄机阁 · 信则有，不信则无</p>
        </div>
    </main>

    <!-- Loading Overlay -->
    <div id="loadingOverlay" class="fixed inset-0 z-40 bg-black/90 flex flex-col items-center justify-center hidden opacity-0 transition-opacity duration-500">
        <div class="taiji-loader mb-8"></div>
        <p class="text-yellow-400 font-artistic text-2xl animate-pulse">正在推演天机...</p>
        <p id="loadingText" class="text-gray-500 text-sm mt-2">排盘计算中</p>
    </div>

    <!-- Result Modal -->
    <div id="resultModal" class="fixed inset-0 z-50 flex items-center justify-center hidden px-4">
        <!-- Backdrop -->
        <div class="absolute inset-0 bg-black/80 backdrop-blur-sm" id="modalBackdrop"></div>
        
        <!-- Modal Content -->
        <div id="modalContent" class="relative bg-gray-900 border border-yellow-600/50 rounded-xl w-full max-w-lg shadow-2xl overflow-hidden transform scale-90 opacity-0 transition-all duration-300">
            
            <!-- Decorative Header -->
            <div class="bg-gradient-to-r from-yellow-900/40 to-gray-900 p-6 text-center border-b border-yellow-600/30 relative overflow-hidden">
                <div class="absolute top-0 left-0 w-full h-1 bg-gradient-to-r from-transparent via-yellow-500 to-transparent"></div>
                <h2 class="text-3xl font-artistic text-yellow-400 text-glow">您的卦象分析结果</h2>
                <p class="text-gray-400 text-xs mt-1">基于生辰八字推演</p>
            </div>

            <!-- Body -->
            <div class="p-6 md:p-8 space-y-6">
                
                <!-- Hexagram Visual -->
                <div class="flex justify-center items-center space-x-8">
                    <!-- Upper Trigram -->
                    <div class="flex flex-col-reverse w-16" id="upperTrigram">
                        <!-- JS will inject lines here -->
                    </div>
                    
                    <!-- Info -->
                    <div class="text-center space-y-2">
                        <h3 id="hexagramName" class="text-2xl font-bold text-white"></h3>
                        <span id="hexagramSymbol" class="text-4xl font-artistic text-yellow-500 block"></span>
                        <div class="inline-block px-3 py-1 rounded-full bg-yellow-900/30 border border-yellow-600/30 text-yellow-200 text-xs" id="elementAttr">
                            五行属性
                        </div>
                    </div>

                    <!-- Lower Trigram -->
                    <div class="flex flex-col-reverse w-16" id="lowerTrigram">
                        <!-- JS will inject lines here -->
                    </div>
                </div>

                <!-- Analysis Text -->
                <div class="bg-white/5 rounded-lg p-4 border-l-4 border-yellow-600">
                    <h4 class="text-yellow-500 font-bold mb-2 flex items-center">
                        <svg class="w-4 h-4 mr-2" fill="none" stroke="currentColor" viewBox="0 0 24 24"><path stroke-linecap="round" stroke-linejoin="round" stroke-width="2" d="M13 16h-1v-4h-1m1-4h.01M21 12a9 9 0 11-18 0 9 9 0 0118 0z"></path></svg>
                        卦象详解
                    </h4>
                    <p id="analysisText" class="text-gray-300 text-sm leading-relaxed text-justify">
                        <!-- Text injected by JS -->
                    </p>
                </div>

                <!-- Fortune Tags -->
                <div class="flex flex-wrap gap-2 justify-center" id="fortuneTags">
                    <!-- Tags injected by JS -->
                </div>
            </div>

            <!-- Footer / Close -->
            <div class="p-4 bg-black/40 text-center border-t border-white/5">
                <button id="closeModalBtn" class="px-8 py-2 rounded-full border border-yellow-600 text-yellow-500 hover:bg-yellow-600 hover:text-black transition-colors duration-300 uppercase text-sm tracking-wider">
                    关闭天机
                </button>
            </div>
        </div>
    </div>

    <script>
        // --- Data & Logic ---

        const trigrams = [
            { name: "乾", symbol: "☰", lines: [1, 1, 1], element: "金", nature: "天" },
            { name: "兑", symbol: "☱", lines: [0, 1, 1], element: "金", nature: "泽" },
            { name: "离", symbol: "☲", lines: [1, 0, 1], element: "火", nature: "火" },
            { name: "震", symbol: "☳", lines: [0, 0, 1], element: "木", nature: "雷" },
            { name: "巽", symbol: "☴", lines: [1, 1, 0], element: "木", nature: "风" },
            { name: "坎", symbol: "☵", lines: [0, 1, 0], element: "水", nature: "水" },
            { name: "艮", symbol: "☶", lines: [1, 0, 0], element: "土", nature: "山" },
            { name: "坤", symbol: "☷", lines: [0, 0, 0], element: "土", nature: "地" }
        ];

        // Simple hash function to generate deterministic numbers from string
        function cyrb53(str, seed = 0) {
            let h1 = 0xdeadbeef ^ seed, h2 = 0x41c6ce57 ^ seed;
            for (let i = 0, ch; i < str.length; i++) {
                ch = str.charCodeAt(i);
                h1 = Math.imul(h1 ^ ch, 2654435761);
                h2 = Math.imul(h2 ^ ch, 1597334677);
            }
            h1 = Math.imul(h1 ^ (h1 >>> 16), 2246822507) ^ Math.imul(h2 ^ (h2 >>> 13), 3266489909);
            h2 = Math.imul(h2 ^ (h2 >>> 16), 2246822507) ^ Math.imul(h1 ^ (h1 >>> 13), 3266489909);
            return 4294967296 * (2097151 & h2) + (h1 >>> 0);
        }

        function generateFortune(name, date, timeIndex) {
            const seedStr = `${name}-${date}-${timeIndex}`;
            const hash = cyrb53(seedStr);
            
            // Determine Trigrams based on hash
            const upperIdx = hash % 8;
            const lowerIdx = (hash >> 4) % 8;
            
            const upper = trigrams[upperIdx];
            const lower = trigrams[lowerIdx];

            // Generate Text
            const moods = ["大吉", "中吉", "小吉", "平", "需谨慎"];
            const mood = moods[hash % moods.length];
            
            const advices = [
                "今日宜静不宜动，修身养性为上策。",
                "机遇暗藏其中，需擦亮双眼，主动出击。",
                "贵人相助，事半功倍，但切记不可骄傲自满。",
                "虽有波折，但终能化险为夷，保持平常心。",
                "财运亨通，但需见好就收，不可贪心。",
                "情感方面需多沟通，避免误会滋生。",
                "事业面临转折，大胆变革方能突破瓶颈。",
                "健康需注意，劳逸结合，饮食清淡。"
            ];
            const advice = advices[hash % advices.length];

            const fullText = `根据您的生辰八字推演，您抽得<b>${upper.nature}上${lower.nature}下</b>之卦。此卦象显示您近期运势<b>${mood}</b>。${advice} 五行属${upper.element}与${lower.element}相生相克，暗示您目前处于能量转换的关键时期，把握当下，顺势而为，必能趋吉避凶。`;

            return {
                upper,
                lower,
                name: `${upper.name}上${lower.name}下`,
                fullName: `${upper.name}${lower.name}`,
                text: fullText,
                mood: mood
            };
        }

        // --- UI Logic ---

        const form = document.getElementById('divinationForm');
        const loadingOverlay = document.getElementById('loadingOverlay');
        const resultModal = document.getElementById('resultModal');
        const modalContent = document.getElementById('modalContent');
        const closeModalBtn = document.getElementById('closeModalBtn');
        const modalBackdrop = document.getElementById('modalBackdrop');

        form.addEventListener('submit', (e) => {
            e.preventDefault();
            
            const name = document.getElementById('userName').value;
            const date = document.getElementById('birthDate').value;
            const time = document.getElementById('birthTime').value;

            if(!name || !date || time === "") return;

            // 1. Show Loading
            loadingOverlay.classList.remove('hidden');
            // Force reflow
            void loadingOverlay.offsetWidth; 
            loadingOverlay.classList.remove('opacity-0');

            // 2. Simulate Calculation Delay
            setTimeout(() => {
                const result = generateFortune(name, date, time);
                renderResult(result);

                // Hide Loading
                loadingOverlay.classList.add('opacity-0');
                setTimeout(() => {
                    loadingOverlay.classList.add('hidden');
                    showModal();
                }, 500);
            }, 2000);
        });

        function renderResult(data) {
            // Set Text
            document.getElementById('hexagramName').innerText = data.fullName;
            document.getElementById('hexagramSymbol').innerText = data.upper.symbol + " " + data.lower.symbol;
            document.getElementById('elementAttr').innerText = `五行: ${data.upper.element} / ${data.lower.element}`;
            document.getElementById('analysisText').innerHTML = data.text;

            // Render Trigram Lines (Top to Bottom visually, but array is 0-2)
            // Upper Trigram is on top (visually first), Lower is below.
            // However, in standard representation, Upper is "Outer", Lower is "Inner".
            // Let's render Upper first (Top), then Lower (Bottom).
            
            renderTrigramLines('upperTrigram', data.upper.lines);
            renderTrigramLines('lowerTrigram', data.lower.lines);

            // Render Tags
            const tagsContainer = document.getElementById('fortuneTags');
            tagsContainer.innerHTML = '';
            const tags = ["事业", "财运", "感情", "健康"];
            const colors = ["bg-blue-900/50 text-blue-200", "bg-yellow-900/50 text-yellow-200", "bg-pink-900/50 text-pink-200", "bg-green-900/50 text-green-200"];
            
            tags.forEach((tag, idx) => {
                const span = document.createElement('span');
                span.className = `px-3 py-1 rounded text-xs border border-white/10 ${colors[idx]}`;
                span.innerText = tag + ": " + (Math.floor(Math.random() * 3) + 3) + "星"; // Random stars for fun
                tagsContainer.appendChild(span);
            });
        }

        function renderTrigramLines(elementId, lines) {
            const container = document.getElementById(elementId);
            container.innerHTML = '';
            // Lines are usually read bottom to top in construction, but displayed top to bottom.
            // Let's reverse the array for display so index 0 is at top.
            [...lines].reverse().forEach(isYang => {
                const div = document.createElement('div');
                div.className = `trigram-line ${isYang ? '' : 'broken'}`;
                if (!isYang) {
                    div.innerHTML = '<span></span><span></span>';
                }
                container.appendChild(div);
            });
        }

        function showModal() {
            resultModal.classList.remove('hidden');
            // Trigger animation
            requestAnimationFrame(() => {
                modalContent.classList.remove('scale-90', 'opacity-0');
                modalContent.classList.add('scale-100', 'opacity-100');
            });
        }

        function hideModal() {
            modalContent.classList.remove('scale-100', 'opacity-100');
            modalContent.classList.add('scale-90', 'opacity-0');
            
            setTimeout(() => {
                resultModal.classList.add('hidden');
            }, 300);
        }

        closeModalBtn.addEventListener('click', hideModal);
        modalBackdrop.addEventListener('click', hideModal);

        // --- Canvas Background Effect (Floating Particles) ---
        const canvas = document.getElementById('particleCanvas');
        const ctx = canvas.getContext('2d');
        let particles = [];

        function resizeCanvas() {
            canvas.width = window.innerWidth;
            canvas.height = window.innerHeight;
        }
        window.addEventListener('resize', resizeCanvas);
        resizeCanvas();

        class Particle {
            constructor() {
                this.x = Math.random() * canvas.width;
                this.y = Math.random() * canvas.height;
                this.size = Math.random() * 2;
                this.speedX = Math.random() * 0.5 - 0.25;
                this.speedY = Math.random() * 0.5 - 0.25;
                this.opacity = Math.random() * 0.5;
            }
            update() {
                this.x += this.speedX;
                this.y += this.speedY;
                if (this.x > canvas.width) this.x = 0;
                if (this.x < 0) this.x = canvas.width;
                if (this.y > canvas.height) this.y = 0;
                if (this.y < 0) this.y = canvas.height;
            }
            draw() {
                ctx.fillStyle = `rgba(255, 215, 0, ${this.opacity})`;
                ctx.beginPath();
                ctx.arc(this.x, this.y, this.size, 0, Math.PI * 2);
                ctx.fill();
            }
        }

        function initParticles() {
            for (let i = 0; i < 50; i++) {
                particles.push(new Particle());
            }
        }

        function animateParticles() {
            ctx.clearRect(0, 0, canvas.width, canvas.height);
            particles.forEach(p => {
                p.update();
                p.draw();
            });
            requestAnimationFrame(animateParticles);
        }

        initParticles();
        animateParticles();

    </script>
</body>
</html>
```
